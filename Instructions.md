## Setup Instructions

### 1. Install DirectX‑Box
Begin by installing **directx-box** using the provided image.

### 2. Create Your Account
During the Ubuntu setup:

- **Account Name:** `xbox`
- **Password:** `xbox`
- Enable **Automatic Login**

This keeps the system feeling more like a console.

### 3. First Launch of Ubuntu
Once Ubuntu finishes installing and you reach the desktop, continue with the steps below.

### 4. Add Xemu to Startup Applications
1. Open **Startup Applications**
2. Click **Add**
3. Enter the following:

**Name:** `Xemu`  
**Command:** `xemu`  
**Comment:** *(optional)*

This makes Xemu launch automatically on boot.

### 5. Restart and Configure Xemu
1. Reboot the system  
2. Wait for Xemu to open automatically  
3. Open **Settings → System**  
4. Configure the required files:

- **Hard Disk:**  
  ```/usr/share/xemu/hdd/xbox_hdd.qcow2```

- **Flash ROM (BIOS):**  
  `/usr/share/xemu/bios/Complex_4627v1.03.bin`

- **MCPX Boot ROM:**  
  `/usr/share/xemu/bios/mcpx_1.0.bin`

After these are set, Xemu will boot like a real Xbox every time the system starts.
