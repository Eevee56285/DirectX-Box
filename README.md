![DirectX Box](https://i.imgur.com/SwdBhdq.png)

### Reimagining the Original Xbox Experience on Modern Hardware

![Status](https://img.shields.io/badge/status-WIP-yellow)
![Platform](https://img.shields.io/badge/platform-Linux-green)
![Emulator](https://img.shields.io/badge/emulator-Xemu-blue)

---

## Download

The current build exceeds GitHub’s 2GB file limit, so the full files can be downloaded here:  
👉 [Download DirectX‑Box Files (OneDrive)](https://1drv.ms/f/c/7d9f2a1e114243b4/IgAHGH-TaaGGTa5xDtIhv-hrAVnw7aFIJ6RJfuxhjB6IbLg?e=NiQOth)

For setup instructions, see:  
👉 [Instructions.md](https://github.com/Eevee56285/DirectX-Box/blob/main/Instructions.md)

---

## What Is DirectX‑Box?

DirectX‑Box is a project aimed at recreating the classic **original Xbox experience** using modern tools.  
The goal isn’t to perfectly clone the original OS, but to capture its:

- Style  
- Personality  
- Atmosphere  
- Dashboard feel  
- Green techno‑organic vibe  

All while running on a flexible Linux foundation.

---

## Dashboard and Interface

The dashboard is the core of DirectX‑Box, powered by **Theseus** — a recreation of the original Xbox dashboard maintained by *MrMilenko*.

Theseus brings back:

- The iconic green glow  
- Original layout  
- Smooth transitions  
- The nostalgic Xbox vibe  

When the system boots, Theseus acts as the main shell, giving DirectX‑Box its identity.

**Note:** This may change. It’s possible to dump an original Xbox hard drive to an image and use the real dashboard. If that becomes the main method, Xemu may be the only component needed for dashboard functionality.

![Dashboard Preview](https://ejosue.com/wp-content/uploads/xbox-menu-screen-1024x575.png)

---

## Game Support and Compatibility

**Xemu** is integrated directly into the system to run original Xbox games.  
Instead of feeling like a separate emulator, Xemu launches seamlessly from the dashboard.

Xemu handles:

- Game compatibility  
- Virtual hard drives  
- Memory units  
- System emulation  
- Smooth performance on modern hardware  

![Xemu Logo](https://th.bing.com/th/id/OIP.eljv8xN4FUcZUn-zNSn6GQAAAA?w=175&h=180&c=7&r=0&o=7&pid=1.7&rm=3)

---

## System Foundation (The Beloved Penguin)

DirectX‑Box runs on **Linux**, which provides:

- Stability  
- Hardware support  
- Flexibility  
- Driver management  
- Performance tuning  

This project currently uses **Ubuntu**, so you’ll see the standard Ubuntu installer and boot screen.

During installation:

- Set the **computer name** to `xbox`  
- Keep all default settings  
- Enable **automatic login** when creating your user account  

![Linux Logo](https://th.bing.com/th/id/OIP.fScYeyQcR7tCKCnqVqHkqQHaHa?w=181&h=181&c=7&r=0&o=7&pid=1.7&rm=3)

---

## Features and Experience

DirectX‑Box aims to feel like a **real console**, not just Linux running an emulator.

Planned features include:

- Full dashboard experience  
- Game launching  
- System menus and settings  
- File browser  
- Theme support  
- Simple developer mode  
- Smooth integration between dashboard and emulator  

The goal is a cohesive, console‑like experience that brings the original Xbox back to life on modern hardware.

---

## Purpose and Inspiration

The original Xbox had a unique style — the green aesthetic, techno‑organic animations, sound effects, and overall vibe.  
DirectX‑Box brings that feeling back using modern hardware.

This is a passion project, not an official recreation.  
It blends nostalgia with modern technology to revive the original Xbox experience while still respecting what made the console iconic.

---

# 🗺️ Roadmap

## **Phase 1 — Foundation (Current)**
- [x] Establish project structure  
- [x] Upload initial build (external hosting due to size)  
- [ ] Improve Xemu auto‑launch integration  
- [ ] Clean up Ubuntu base image  
- [ ] Add a custom Xbox‑style boot animation  

## **Phase 2 — Dashboard Integration**
- [ ] Integrate Theseus as primary shell  
- [ ] Add theme support (green, crystal, debug‑kit themes)  
- [ ] Implement system settings UI  
- [ ] Add file browser with Xbox‑style UI  
- [ ] Add “Developer Mode” toggle  

## **Phase 3 — Game Experience**
- [ ] Seamless game launching from dashboard  
- [ ] Virtual memory unit support  
- [ ] Improved controller mapping presets  
- [ ] Auto‑scan for installed games  
- [ ] Optional “Classic Xbox Sounds” pack  

## **Phase 4 — System Polish**
- [ ] Custom DirectX‑Box updater  
- [ ] Optional desktop mode switcher  
- [ ] Performance tuning for low‑end hardware  
- [ ] Accessibility improvements  
- [ ] Documentation, screenshots, and video demos  

## **Long‑Term / Stretch Goals**
- [ ] Support for dumping original Xbox HDDs  
- [ ] Optional real‑hardware compatibility (if future drives support Xbox discs)  
- [ ] Community theme marketplace  

---

# ❓ FAQ

### **What is DirectX‑Box?**
A Linux‑based system designed to recreate the look and feel of the original Xbox dashboard.

### **Is this an emulator?**
Not exactly.  
DirectX‑Box uses **Xemu** for game compatibility, but the goal is to make the entire system feel like a real console.

### **Does this use the real Xbox OS?**
Currently it uses **Theseus**, but future builds may support using a dumped original Xbox HDD image for a more authentic dashboard.

### **Can it read real Xbox discs?**
Not with modern disc drives. If someone eventually creates a drive capable of reading Xbox discs, support may be added in the future.

### **What hardware does it run on?**
Anything that can run Ubuntu reliably:
- Laptops  
- Desktops  
- Mini PCs  
- Some handheld PCs  

### **Is this legal?**
DirectX‑Box itself is legal.  
Users are responsible for legally obtaining their own game files or BIOS dumps.

### **When will development continue?**
Full development begins this summer.

### **Can I contribute?**
Yes! Contributions, ideas, and testing feedback are welcome once the first public build is ready.

---

# Project Status

Development will begin over the summer.  
Until then, this GitHub page will serve as the main project hub.

---

# Todo List

- [x] Start the project  
- [ ] Fix Xemu integration and make it auto‑launch (in development)  
- [ ] Disc compatibility — unlikely due to modern disc‑drive limitations.  
      If someone creates a drive that can read Xbox discs, support may be added in the future.
