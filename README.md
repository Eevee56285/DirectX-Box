# DirectX‑Box

The current build exceeds GitHub’s 2GB file limit, so the full files can be downloaded here:  
[**Download DirectX‑Box Files (OneDrive)**](https://1drv.ms/f/c/7d9f2a1e114243b4/IgAHGH-TaaGGTa5xDtIhv-hrAVnw7aFIJ6RJfuxhjB6IbLg?e=NiQOth)

DirectX‑Box is a project aimed at recreating the classic **original Xbox experience** using modern tools. The goal isn’t to perfectly clone the original OS, but to capture its **style, personality, and atmosphere** while running on a Linux foundation.  
For setup instructions, see:  
👉 [**Instructions.md**](https://github.com/Eevee56285/DirectX-Box/blob/main/Instructions.md)

---

## Dashboard and Interface

The dashboard is the core of DirectX‑Box, powered by **[Theseus](https://github.com/MrMilenko/Theseus)** — a recreation of the original Xbox dashboard maintained by *MrMilenko*. Theseus brings back the iconic green glow, transitions, layout, and overall vibe that defined the original console.

When the system boots, Theseus acts as the main shell, giving DirectX‑Box its identity while still allowing room for future expansion.

> **Note:** This may change. I recently discovered that it’s possible to dump an original Xbox OS to a hard‑drive image. If that becomes the main method, Xemu may be the only component needed for dashboard functionality.

![Dashboard Preview](https://ejosue.com/wp-content/uploads/xbox-menu-screen-1024x575.png)

---

## Game Support and Compatibility

**[Xemu](https://xemu.app/)** is integrated directly into the system to run original Xbox games. Instead of feeling like a separate emulator, Xemu launches seamlessly from the dashboard so the experience feels unified.

Xemu handles:
- Game compatibility  
- Virtual hard drives  
- Memory units  
- System emulation  
- Smooth performance on modern hardware  

![Xemu Logo](https://th.bing.com/th/id/OIP.eljv8xN4FUcZUn-zNSn6GQAAAA?w=175&h=180&c=7&r=0&o=7&pid=1.7&rm=3)

---

## System Foundation (The Beloved Penguin)

DirectX‑Box runs on **Linux**, which provides stability, hardware support, and flexibility. Linux manages drivers, performance, and background processes, allowing the dashboard and Xemu to work together smoothly.

This project currently uses **Ubuntu**, so you’ll see the Ubuntu installer and boot screen. During installation:

- Set the **system name** to `xbox`  
- Keep all default settings  
- Enable **automatic login** when creating your password  

![Linux Logo](https://th.bing.com/th/id/OIP.fScYeyQcR7tCKCnqVqHkqQHaHa?w=181&h=181&c=7&r=0&o=7&pid=1.7&rm=3)

---

## Features and Experience

DirectX‑Box aims to feel like a **real console**, not just Linux running an emulator. Planned features include:

- Full dashboard experience  
- Game launching  
- System menus and settings  
- File browser  
- Theme support  
- Simple developer mode  
- Smooth integration between dashboard and emulator  

The goal is a cohesive, console‑like experience that brings the original Xbox back to life.

---

## Purpose and Inspiration

The original Xbox had a unique style — the green aesthetic, the techno‑organic animations, the sound effects, the whole vibe. DirectX‑Box is a way to bring that feeling back using modern hardware.

This is a passion project, not an official recreation. It mixes nostalgia with modern tech to revive the original Xbox experience while respecting what made it special.

---

## Project Status

Development will begin over the summer. Until then, this GitHub page will serve as the main project hub.

---

## Todo List

- [x] Start the project  
- [ ] Fix Xemu integration and make it auto‑launch (in development)  
- [ ] Disc compatibility — **unlikely** due to modern disc drive limitations.  
      If someone creates a drive that can read Xbox discs, support *may* be added in the future.
