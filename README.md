<p align="center">
  <img src="assets/screenshots/ventoy.png" alt="Ventoy Toolkit Hero" width="800">
</p>

# Ventoy Toolkit

A professional, high-performance multiboot USB toolkit designed for system administrators, developers, and security professionals. This repository contains the complete configuration for a modular boot environment, enabling seamless deployment of multiple operating systems, recovery tools, and diagnostic utilities from a single USB drive.

<p align="center">
  <img src="https://img.shields.io/badge/Ventoy-1.0.99-blue?logo=ventoy" alt="Ventoy">
  <img src="https://img.shields.io/badge/Arch_Linux-Rolling-blue?logo=arch-linux" alt="Arch Linux">
  <img src="https://img.shields.io/badge/Kali_Linux-2025.4-blueviolet?logo=kali-linux" alt="Kali Linux">
  <img src="https://img.shields.io/badge/NixOS-Declarative-7E7EFF?logo=nixos" alt="NixOS">
  <img src="https://img.shields.io/badge/Windows-Recovery-0078D6?logo=windows" alt="Windows">
  <img src="https://img.shields.io/badge/SystemRescue-Stable-orange?logo=linux" alt="SystemRescue">
  <img src="https://img.shields.io/badge/Clonezilla-Disk_Imaging-27ae60?logo=linux" alt="Clonezilla">
  <img src="https://img.shields.io/badge/GParted-Partitioning-orange?logo=linux" alt="GParted">
  <img src="https://img.shields.io/badge/MemTest86+-Hardware-red?logo=linux" alt="MemTest86+">
  <img src="https://img.shields.io/badge/Tails-Privacy-purple?logo=tails" alt="Tails">
</p>

---

## Core Components

- [**Ventoy Official Website**](https://www.ventoy.net)
- [**Ventoy GitHub Repository**](https://github.com/ventoy/Ventoy)

---

## Project Structure

The toolkit is organized into logical directories to ensure scalability and ease of maintenance.

```text
/
├── assets/                 # Repository visual assets and logos
│   └── screenshots/        # Tool and OS environment captures
├── iso/                    # ISO storage directory
│   ├── rescue/             # Specialized recovery environments
│   └── tools/              # Utility-focused distributions
└── ventoy/                 # Ventoy core configuration
    └── ventoy/
        ├── ventoy.json      # Global settings, persistence, and aliases
        └── theme/           # Custom GRUB boot theme (Squid)
```

---

## Toolkit Content

### Primary Operating Systems

#### <img src="assets/arch.png" width="24"> Arch Linux
A minimalist, lightweight, and highly customizable Linux distribution. Ideal for power users who require a lean environment.

- **ISO**: `archlinux-x86_64.iso`
- **Documentation**: [Official Wiki](https://wiki.archlinux.org/)
- **Download**: [Official Release](https://archlinux.org/download/)

![Arch Linux Screenshot](assets/screenshots/arch.png)

---

#### <img src="assets/kali.png" width="24"> Kali Linux
The professional standard for advanced Penetration Testing and Security Auditing. Configured with a dedicated persistence file.

- **ISO**: `kali-linux-live.iso`
- **Persistence**: `kali-persistence.dat`
- **Documentation**: [Official Docs](https://www.kali.org/docs/)
- **Download**: [Get Kali](https://www.kali.org/get-kali/)

![Kali Linux Screenshot](assets/screenshots/kali.png)

---

#### <img src="assets/nixos.png" width="24"> NixOS
A declarative Linux distribution built on the Nix package manager, offering reproducible builds and reliable rollbacks.

- **ISO**: `nixos-graphical-*.iso`
- **Documentation**: [Official Manual](https://nixos.org/manual/)
- **Download**: [NixOS Download](https://nixos.org/download.html)

![NixOS Screenshot](assets/screenshots/nixos.png)

---

### Recovery & Specialized Tools

#### <img src="assets/windows.png" width="24"> Hiren's BootCD PE
A Windows 10 PE based emergency boot disk loaded with recovery tools, partitioning software, and antivirus utilities.

- **ISO**: `HBCD_PE_x64.iso`
- **Download**: [HBCD Official Website](https://www.hirensbootcd.org/download/)

![Windows PE Screenshot](assets/screenshots/windows.png)

---

#### <img src="assets/rescue.png" width="24"> SystemRescue
A Linux system rescue disk available as a bootable CD-ROM or USB stick for administrating or repairing your system and data after a crash.

- **ISO**: `iso/rescue/systemrescue.iso`
- **Download**: [SystemRescue Download](https://www.system-rescue.org/Download/)

![SystemRescue Screenshot](assets/screenshots/rescue.png)

---

#### <img src="assets/clonezilla.png" width="24"> Clonezilla
A partition and disk imaging/cloning program similar to Symantec Ghost. Perfect for system backup and massive deployment.

- **ISO**: `iso/tools/clonezilla.iso`
- **Download**: [Clonezilla Downloads](https://clonezilla.org/downloads.php/)

![Clonezilla Screenshot](assets/screenshots/clonezilla.png)

---

#### <img src="assets/gparted.png" width="24"> GParted
A free partition editor for graphically managing your disk partitions. Resize, copy, and move partitions without data loss.

- **ISO**: `iso/tools/gparted.iso`
- **Download**: [GParted Download](https://gparted.org/download.php)

![GParted Screenshot](assets/screenshots/gparted.png)

---

#### <img src="assets/memtest.png" width="24"> MemTest86+
An open-source standalone memory tester for x86 and x86-64 architecture computers.

- **ISO**: `iso/tools/memtest.iso`
- **Download**: [MemTest86+ Website](https://memtest.org/)

![MemTest86+ Screenshot](assets/screenshots/memtest.png)

---

#### <img src="assets/tails.png" width="24"> Tails
The Amnesic Incognito Live System. A security-focused Debian-based Linux distribution aimed at preserving privacy and anonymity.

- **ISO**: `iso/tools/tails.iso`
- **Documentation**: [Tails Documentation](https://tails.net/doc/)
- **Download**: [Install Tails](https://tails.net/install/)

![Tails Screenshot](assets/screenshots/tails.png)

---

---

<p align="center">
  Generated by <b>Ventoy Toolkit Manager</b>
</p>
