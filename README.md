<p align="center">
  <img src="assets/hero.png" alt="Ventoy Toolkit Hero" width="800">
</p>

# Ventoy Toolkit

> A professional multiboot USB toolkit for system administrators, developers, and security enthusiasts.

[![Ventoy](https://img.shields.io/badge/Ventoy-1.0.99-blue?logo=ventoy)](https://www.ventoy.net)
[![Arch Linux](https://img.shields.io/badge/Arch_Linux-Rolling-blue?logo=arch-linux)](https://archlinux.org/)
[![Kali Linux](https://img.shields.io/badge/Kali_Linux-2025.4-blueviolet?logo=kali-linux)](https://www.kali.org/)
[![NixOS](https://img.shields.io/badge/NixOS-Declarative-7E7EFF?logo=nixos)](https://nixos.org/)
[![Privacy](https://img.shields.io/badge/Privacy-Tails-purple?logo=tails)](https://tails.net/)

---

## Table of Contents

- [Overview](#overview)
- [Toolkit Content](#toolkit-content)
- [Project Structure](#project-structure)
- [Custom Features](#custom-features)
- [Official Links](#official-links)

---

## Overview

Ta clé est un **multiboot toolkit** ultra-complet permettant de démarrer directement des fichiers ISO sans flashage à chaque utilisation. Elle est organisée pour répondre à tous les besoins : installation d'OS, dépannage Windows, forensic, pentesting et maintenance système.

| Catégorie | Outils |
| :--- | :--- |
| **OS** | Arch Linux, Kali Linux, NixOS |
| **Windows / Recovery** | Hiren's BootCD PE |
| **Rescue** | SystemRescue |
| **Disk Management** | Clonezilla, GParted |
| **Hardware Diagnostic** | MemTest86+ |
| **Privacy & Anonymity** | Tails |

---

## Toolkit Content

### Primary Systems

| Tool | Description | ISO Filename |
| :--- | :--- | :--- |
| **Arch Linux** | Minimalist rolling release distribution. | `archlinux-x86_64.iso` |
| **Kali Linux** | Offensive security & pentesting (Persistent). | `kali-linux-live.iso` |
| **NixOS** | Declarative configuration-based OS. | `nixos-graphical-*.iso` |

### Rescue & Tools

| Tool | Category | Key Features |
| :--- | :--- | :--- |
| **Hiren's BootCD PE** | Windows Recovery | Antivirus, Partitioning, Password Reset |
| **SystemRescue** | Linux Rescue | Boot repair, Filesystem recovery |
| **Clonezilla** | Disk Imaging | Disk cloning and massive deployment |
| **GParted** | Partitioning | Live partition editor (resize/move/repair) |
| **MemTest86+** | RAM Diagnostic | Hardware level memory testing |
| **Tails** | Privacy | Amnesic OS with Tor integrated |

---

## Project Structure

```text
/
├── assets/                 # Repository visual assets
│   └── hero.png
├── iso/                    # Main ISO storage
│   ├── archlinux-x86_64.iso
│   ├── kali-linux-live.iso
│   ├── nixos-graphical.iso
│   ├── HBCD_PE_x64.iso
│   ├── rescue/             # Rescue specific ISOs
│   │   └── systemrescue.iso
│   └── tools/              # Utilities & Tools
│       ├── clonezilla.iso
│       ├── gparted.iso
│       ├── memtest.iso
│       └── tails.iso
└── ventoy/                 # Ventoy configuration
    └── ventoy/
        ├── ventoy.json      # Theme, persistence, and alias config
        └── theme/           # Custom GRUB theme
```

---

## Custom Features

Ton setup n'est pas qu'une simple liste de fichiers. Il inclut des fonctionnalités avancées configurées dans `ventoy.json` :

*   **Custom Theme** : Thème "Squid" premium pré-installé.
*   **Custom Icons** : Icônes dédiées pour chaque OS (Arch, Kali, NixOS, Windows).
*   **Menu Aliases** : Noms de fichiers ISO renommés proprement dans le menu de boot.
*   **Kali Persistence** : Sauvegarde tes modifications sur Kali (`kali-persistence.dat`).
*   **Logic Organization** : Dossiers `/rescue` et `/tools` pour un menu propre.

---

## Official Links

### OS & ISOs
- [**Arch Linux**](https://archlinux.org/download/) - [Doc](https://wiki.archlinux.org/)
- [**Kali Linux**](https://www.kali.org/get-kali/) - [Doc](https://www.kali.org/docs/)
- [**NixOS**](https://nixos.org/download.html) - [Doc](https://nixos.org/manual/)
- [**Hiren's BootCD PE**](https://www.hirensbootcd.org/download/)
- [**SystemRescue**](https://www.system-rescue.org/Download/)
- [**Clonezilla**](https://clonezilla.org/downloads.php/)
- [**GParted**](https://gparted.org/download.php)
- [**MemTest86+**](https://memtest.org/)
- [**Tails**](https://tails.net/install/) - [Doc](https://tails.net/doc/)

### Bootloader
- [**Ventoy Official Website**](https://www.ventoy.net)
- [**Ventoy GitHub**](https://github.com/ventoy/Ventoy)

---

<p align="center">
  Generated with by <b>Ventoy Toolkit Manager</b>
</p>
