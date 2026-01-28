# Mithl-OS
![Mithl-OS Logo](OSLogo.png)
> **The Modern Operating System for Creators**

![Fast. Beautiful. Yours.](https://img.shields.io/badge/Status-Active%20Development-00d4ff?style=for-the-badge)
![License](https://img.shields.io/badge/License-Open%20Source-ffeb3b?style=for-the-badge)

---

## 🚀 What is Mithl-OS?

**Mithl-OS** is a high-performance, independent operating system built from scratch with a singular vision: **Speed, Aesthetics, and Control**. Unlike traditional operating systems that carry decades of legacy code, Mithl-OS is designed from the ground up to be your reliable daily driver for creative work and development.

We believe an operating system should be **invisible**—it should get out of your way, boot instantly, run efficiently, and provide a distraction-free environment for you to build *your* projects.

---

## ⚡ Core Philosophy

### Performance First
- **Direct-to-Metal Graphics**: Custom graphics pipeline that renders directly to the framebuffer for zero input lag
- **Optimized Memory Management**: Rewritten memory scheduler that reduces fragmentation by 40%
- **Instant Boot**: Optimized boot sequence that launches directly into the graphical environment
- **Zero Bloat**: No background telemetry, no unnecessary services, just pure performance

### Rock Solid Stability
- **Micro-kernel Inspired Architecture**: Isolates drivers for maximum uptime and system stability
- **Robust Process Management**: Advanced scheduling and memory management for smooth multitasking
- **Crash Isolation**: System-critical components are protected from application failures

### Beautiful by Design
- **Glass Prism UI**: A cohesive, glassmorphic design language that looks stunning on any display
- **Distraction-Free Workspace**: No notifications, no ads, no interruptions—just your work
- **Consistent Design System**: Every element follows the same visual language for a unified experience

---

## 🎯 Key Features

### 🖥️ Custom Kernel
Built from scratch in C with performance-critical components optimized in assembly:
- **Custom Memory Manager**: Efficient allocation and deallocation with minimal fragmentation
- **Advanced Scheduler**: Fair scheduling with support for real-time tasks
- **Virtual File System (VFS)**: Unified interface for multiple filesystem types (FAT32, MNFS, RamFS)
- **Hardware Abstraction Layer**: Clean separation between hardware and software

### 🎨 Teal UI Desktop Environment
A modern, glass-morphic desktop environment:
- **Custom Window Manager**: Smooth window management with compositing effects
- **Built-in Applications**: File Manager, Terminal, Text Editor, Calculator, Settings, and more
- **Integrated Graphics**: Direct framebuffer access for maximum performance
- **Mouse & Keyboard Support**: Full input device support with custom drivers

### 🛠️ Developer Tools
Full development environment included:
- **GCC/G++ Support**: Compile and run C/C++ projects natively
- **TCC Compiler**: Tiny C Compiler integrated for fast compilation
- **POSIX-like Environment**: Familiar Unix-style commands and utilities
- **Standard Toolchain**: Make, linker, and essential build tools

### 🎮 Entertainment
- **DOOM**: Yes, it runs DOOM! Classic gaming on a modern OS
- **Multimedia Support**: Image viewer and media capabilities

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────┐
│         User Applications               │
│  (Shell, File Manager, Calculator...)   │
└─────────────────┬───────────────────────┘
                  │ System Calls
┌─────────────────▼───────────────────────┐
│          Mithl Kernel (Ring 0)          │
│  ┌──────────┬──────────┬──────────┐    │
│  │   VFS    │  Memory  │ Graphics │    │
│  │ Manager  │ Manager  │  Driver  │    │
│  └──────────┴──────────┴──────────┘    │
└─────────────────┬───────────────────────┘
                  │ Hardware Access
┌─────────────────▼───────────────────────┐
│            Hardware Layer               │
│    (CPU, RAM, Disk, GPU, Devices)      │
└─────────────────────────────────────────┘
```

The streamlined architecture ensures minimal overhead and maximum performance.

---

## 📦 What's Included

### System Components
- **Kernel**: Custom x86 kernel with multiboot2 support
- **Bootloader**: GRUB2 for reliable booting
- **Desktop Environment**: Complete GUI with window manager and compositor
- **Device Drivers**: Keyboard, mouse, VGA, ATA disk, RTC, and more

### Applications
- **System Utilities**: ls, ps, cat, mkdir, cp, mv, and more
- **GUI Applications**: 
  - File Manager with icon support
  - Terminal emulator
  - Text Editor (Notepad)
  - Calculator
  - Settings panel
  - Task Manager
  - Dashboard
  - Image Viewer
  - Clock

### Development Tools
- **Compilers**: GCC, G++, TCC
- **Build System**: Make, custom linker
- **Libraries**: Custom libc implementation
- **Headers**: Standard C headers and TCC includes

---

## 🚀 Getting Started

### Download Latest Release

Mithl-OS releases are available through our public distribution repository:

**📦 Distribution Repository**: [https://github.com/DoguparthiAakash/Mithl/releases](https://github.com/DoguparthiAakash/Mithl/releases)

This repository contains:
- ✅ Latest ISO builds (ready to run)
- ✅ Release notes and changelogs
- ✅ Documentation and user guides
- ✅ Pre-built binaries

### Quick Start

**1. Download the Latest ISO**
```bash
# Visit the releases page
https://github.com/DoguparthiAakash/Mithl/releases

# Or clone the distribution repository
git clone https://github.com/DoguparthiAakash/Mithl.git
cd Mithl
```

**2. Run in QEMU (Emulator)**
```bash
qemu-system-x86_64 -cdrom iso/Mithl-latest.iso -m 512M
```

**3. Write to USB Drive (Real Hardware)**
```bash
# ⚠️ Replace /dev/sdX with your USB device
sudo dd if=iso/Mithl-latest.iso of=/dev/sdX bs=4M status=progress
sudo sync
```

The OS will boot and you'll see the beautiful Teal UI desktop environment!

### For Developers

> **Note**: The main Mithl-OS codebase is maintained in a private repository to ensure code quality and security. 

**Interested in contributing to the source code?** Apply for contributor access through our contribution form on the website or email us at [doguparthiaakash@gmail.com](mailto:doguparthiaakash@gmail.com).

Approved contributors will receive:
- 🔑 Access to the private development repository
- 📚 Developer documentation and onboarding materials
- 👥 Invitation to the core development team
- 🎯 Guidance on where to start contributing

---

## 🗺️ Roadmap

### ✅ Completed (v0.5)
- ✅ Stable kernel with improved memory management
- ✅ Glass Prism UI design system
- ✅ Full GUI application suite
- ✅ TCC compiler integration
- ✅ DOOM game port
- ✅ Userspace process support

### 🚧 In Progress
- 🔨 Network stack implementation
- 🔨 USB driver support
- 🔨 Audio subsystem
- 🔨 Multi-core CPU support

### 🔮 Future (Experimental)
- 🌟 **Project Curiosity**: Optional offline AI assistance for developers
- 🌟 Advanced window tiling and workspace management
- 🌟 Package manager for third-party applications
- 🌟 UEFI boot support
- 🌟 64-bit kernel transition

---

## 🤝 Contributing

We're building the future of operating systems, and we need passionate developers, designers, and creators to join us!

### Areas We Need Help With

**🛠️ Kernel Development**
- Memory management optimization
- Process scheduler improvements
- Device driver development
- Filesystem implementations

**🎨 UI/UX Design**
- Glass Prism theme refinements
- New application designs
- Icon and asset creation
- Animation and transitions

**📚 Documentation**
- API documentation
- User guides and tutorials
- Code comments and explanations
- Architecture documentation

**🔧 Application Development**
- New userspace applications
- Porting existing software
- Game development
- Productivity tools

### How to Contribute

Mithl-OS development happens in a **private repository** to maintain code quality, security, and focused development. We carefully select contributors who are passionate about OS development.

#### 🎯 Application Process

**Step 1: Submit Your Application**

Visit our website and fill out the contribution form, or send an email to [doguparthiaakash@gmail.com](mailto:doguparthiaakash@gmail.com)

**Required Information:**
- Full name and email address
- GitHub username
- Area of expertise (Kernel, UI/UX, Drivers, Applications, Documentation)
- Relevant experience and skills
- What you'd like to contribute
- Why you're interested in Mithl-OS
- Links to previous work (GitHub repos, portfolio, etc.)

**Step 2: Review Process**

Our team will review your application within 3-5 business days. We look for:
- ✅ Relevant technical skills
- ✅ Passion for systems programming
- ✅ Alignment with project goals
- ✅ Previous open-source contributions (preferred but not required)

**Step 3: Onboarding**

Approved contributors receive:
- 🔑 **Private Repository Access**: Invitation to the main Mithl-OS codebase
- 📚 **Developer Documentation**: Architecture guides, coding standards, and API references
- 👥 **Team Invitation**: Join our development team on GitHub
- 💬 **Communication Channels**: Access to developer discussions and planning
- 🎯 **First Tasks**: Guided issues to help you get started

#### 📧 Quick Apply

**Email**: [doguparthiaakash@gmail.com](mailto:doguparthiaakash@gmail.com)  
**Subject**: Contribution Application - [Your Area of Interest]

Or use the contribution form on our website: [https://doguparthiaakash.github.io/Mithl/contribute.html](https://doguparthiaakash.github.io/Mithl/contribute.html)

---

## 📄 License

Mithl-OS is open-source software. Please refer to the LICENSE file in the repository for details.

---

## 🔗 Links

- **Website**: [https://doguparthiaakash.github.io/Mithl/](https://doguparthiaakash.github.io/Mithl/)
- **Distribution Repository**: [https://github.com/DoguparthiAakash/Mithl/releases](https://github.com/DoguparthiAakash/Mithl/releases)
- **Contribute**: [doguparthiaakash@gmail.com](mailto:doguparthiaakash@gmail.com)
- **Contribution Form**: [https://doguparthiaakash.github.io/Mithl/contribute.html](https://doguparthiaakash.github.io/Mithl/contribute.html)

---

## 🌟 Why Mithl-OS?

In a world dominated by closed-source operating systems and bloated Linux distributions, Mithl-OS offers something different:

- **True Independence**: Not based on Linux or any existing OS
- **Performance Focused**: Every line of code is optimized for speed
- **Beautiful Design**: Aesthetics are not an afterthought
- **Developer Friendly**: Built by developers, for developers
- **Transparent**: Fully open-source, no hidden telemetry
- **Educational**: Learn OS development from a real, working system

---

## 💡 Philosophy

> "An operating system should be invisible. It should boot instantly, run efficiently, and get out of your way so you can focus on what matters—your work, your creativity, your projects."

Mithl-OS is built on the principle that software should serve the user, not the other way around. We reject the notion that you must accept bloat, telemetry, and complexity in exchange for functionality.

---

## 🎓 Learn More

Want to understand how Mithl-OS works? Check out:
- **Architecture Documentation**: See how the kernel, memory manager, and graphics system work together
- **API Reference**: Learn how to write applications for Mithl-OS
- **Build System**: Understand the compilation and linking process
- **Contributing Guide**: Get started with your first contribution

---

*Mithl-OS: Fast. Beautiful. Yours.*

**Built with ❤️ by developers who believe in technological sovereignty**
