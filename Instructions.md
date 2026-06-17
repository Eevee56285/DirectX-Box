INSTRUCTIONS FOR AUTO‑STARTING XEMU ON UBUNTU (WITH FIXES)

1. REQUIREMENTS
- Xemu must launch normally when run manually using the command: xemu
- Your virtual machine must have 3D acceleration enabled.
- Ubuntu must have the correct graphics drivers installed.

2. ENABLE 3D ACCELERATION IN VMWARE
1. Shut down the VM completely.
2. Open VMware Player → Settings → Display.
3. Enable “Accelerate 3D graphics”.
4. Set graphics memory to 2 GB or more.
5. Set renderer to Automatic or DirectX 11.

Install VMware tools inside Ubuntu:

sudo apt install open-vm-tools-desktop -y
sudo reboot

3. FIX XEMU FILE PERMISSIONS
If Xemu crashes with “Permission denied”, fix ownership of its files:

sudo chown -R $USER:$USER /usr/share/xemu
sudo chmod -R 755 /usr/share/xemu

4. REMOVE DUPLICATE AUTOSTART ENTRIES
Delete GNOME autostart:

rm ~/.config/autostart/xemu.desktop

Disable any generated autostart service:

systemctl --user disable app-xemu@autostart.service
systemctl --user daemon-reload

5. CREATE A USER-LEVEL SYSTEMD SERVICE
Create the service:

systemctl --user edit --full xemu.service

Paste this:

[Unit]
Description=Auto-start Xemu
After=graphical-session.target

[Service]
Type=simple
ExecStart=/usr/bin/xemu
Restart=on-failure
RestartSec=2
Environment=DISPLAY=:0
Environment=XAUTHORITY=/home/USERNAME/.Xauthority
Environment=WAYLAND_DISPLAY=
Environment=GDK_BACKEND=x11

[Install]
WantedBy=default.target

Replace USERNAME with your actual username.

Save and exit.

6. ENABLE AND START THE SERVICE

systemctl --user daemon-reload
systemctl --user enable xemu.service
systemctl --user start xemu.service

Check status:

systemctl --user status xemu.service

You want to see: active (running)

------------------------------------------------------------
TROUBLESHOOTING
------------------------------------------------------------

ISSUE 1: Xemu exits immediately with “status=1/FAILURE”
Check logs:

journalctl --user -u xemu.service --no-pager --lines=50

If you see “Permission denied”, fix permissions:

sudo chown -R $USER:$USER /usr/share/xemu
sudo chmod -R 755 /usr/share/xemu

ISSUE 2: “Could not open xbox_hdd.qcow2”
Fix HDD permissions:

sudo chown -R $USER:$USER /usr/share/xemu/hdd
sudo chmod -R 755 /usr/share/xemu/hdd

ISSUE 3: Xemu won’t launch inside VMware
Check OpenGL version:

glxinfo | grep "OpenGL version"

You need OpenGL 3.3 or higher.

If missing:

sudo apt install open-vm-tools-desktop -y
sudo reboot

ISSUE 4: Xemu works manually but not from systemd
Make sure the service file includes:

Environment=DISPLAY=:0
Environment=XAUTHORITY=/home/USERNAME/.Xauthority
Environment=GDK_BACKEND=x11

ISSUE 5: You are using Wayland
Xemu works best on X11.

Log out → click the gear icon → choose “Ubuntu on Xorg”.

ISSUE 6: Xemu opens, closes, then reopens
This is caused by Restart=always.
Fix by changing it to:

Restart=on-failure

ISSUE 7: Xemu is still running in the background
Stop the service:

systemctl --user stop xemu.service

Kill leftover processes:

pkill xemu

------------------------------------------------------------
OPTIONAL SETTINGS
------------------------------------------------------------

Start Xemu fullscreen:
ExecStart=/usr/bin/xemu -full-screen

Auto-load a game:
ExecStart=/usr/bin/xemu -full-screen -dvd_path "/path/to/game.iso"

------------------------------------------------------------
END OF FILE
------------------------------------------------------------
