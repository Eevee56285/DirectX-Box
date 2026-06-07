# DirectX-Box

DirectX-Box is a project focused on recreating the classic Xbox experience using modern tools. The goal is to bring back the feeling of turning on the original Xbox, but in a way that works on today’s hardware and isn’t limited by the old system’s restrictions. Instead of trying to perfectly copy the original Xbox operating system, this project focuses on capturing its style, personality, and atmosphere while running on a Linux foundation.

## Dashboard and Interface

The dashboard is the heart of DirectX-Box, built around the [Theseus](https://github.com/MrMilenko/Theseus "Theseus")
 original xbox os maintained by MrMilenko. This is what gives the system its identity. Theseus recreates the look and feel of the original Xbox dashboard, including the green glow, the layout, the transitions, and the overall vibe that made the console so memorable. When the system boots, Theseus is the first thing you see, and it becomes the main way you navigate everything. It acts as the shell of the system, giving DirectX-Box the same energy and style that defined the original console, while still being flexible enough to grow and evolve over time.

![Dashboard Preview](https://ejosue.com/wp-content/uploads/xbox-menu-screen-1024x575.png)

## Game Support and Compatibility

[Xemu](https://www.bing.com/ck/a?!&&p=505710e26b7f3b87264e9b79292320b1ee71c81d89d4bf5e651906563780f99fJmltdHM9MTc4MDc5MDQwMA&ptn=3&ver=2&hsh=4&fclid=22ee684d-f339-67fb-33bc-7eb9f2d16651&psq=xemu&u=a1aHR0cHM6Ly94ZW11LmFwcC8 "Xemu")
 is the component responsible for running original Xbox games. Instead of being treated like a separate emulator, it is integrated directly into the system so that launching a game feels natural and connected to the dashboard. When a game is selected from the interface, it opens through Xemu, but the goal is for it to feel like part of the system rather than a separate program. Xemu handles the game compatibility, the virtual hard drive, memory units, and everything else needed to make original Xbox titles run smoothly on modern hardware.

![Xemu Logo](https://th.bing.com/th/id/OIP.eljv8xN4FUcZUn-zNSn6GQAAAA?w=175&h=180&c=7&r=0&o=7&pid=1.7&rm=3)

## System Foundation (the beloved penguin)

Linux serves as the base layer that keeps everything stable and functional. It manages the hardware, drivers, performance, and background processes that allow the dashboard and Xemu to work together without issues. Using Linux also makes the project flexible, since it can run on different types of hardware without needing to be rebuilt from scratch. It also allows the system to switch between the Xbox-style dashboard and a normal desktop environment whenever deeper customization or development work is needed.

![linux logo](https://th.bing.com/th/id/OIP.fScYeyQcR7tCKCnqVqHkqQHaHa?w=181&h=181&c=7&r=0&o=7&pid=1.7&rm=3)

## Features and Experience

DirectX-Box is designed to feel like a real console rather than just a Linux machine running an emulator. It includes a full dashboard experience, game launching, system menus, settings, a file browser, theme support, and a simple developer mode for experimenting with the system. The goal is to create something that feels complete and cohesive, where every part of the system works together to recreate the classic Xbox experience in a modern way.

## Purpose and Inspiration

The original Xbox had a very distinct style that set it apart from other consoles. The green aesthetic, the animations, the sound effects, and the overall “techno-organic” vibe gave it a personality that still stands out today. DirectX-Box is a way to bring that feeling back using modern tools. It isn’t meant to be official or perfect. It’s a personal project that mixes nostalgia with modern technology, giving the original Xbox experience a new life on today’s hardware while still respecting what made the original system special.

## Todo List
- [ ] Start making it with linux
- [ ] Disc compatibility will never come to this operating system just becuase of the current disc drive if someone later makes a compatible drive with xbox discs i might bring compatibility to the operating sytem
