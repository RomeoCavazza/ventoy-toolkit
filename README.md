<p align="center">
  <img src="assets/hero.png" alt="Ventoy Toolkit Hero" width="800">
</p>

# Ventoy Toolkit

> A professional multiboot USB toolkit for system administrators, developers, and security enthusiasts.

<p align="center">
  <img src="https://img.shields.io/badge/Ventoy-1.0.99-blue?style=for-the-badge&logo=ventoy" alt="Ventoy">
  <img src="https://img.shields.io/badge/Arch_Linux-Rolling-blue?style=for-the-badge&logo=arch-linux" alt="Arch Linux">
  <img src="https://img.shields.io/badge/Kali_Linux-2025.4-blueviolet?style=for-the-badge&logo=kali-linux" alt="Kali Linux">
  <img src="https://img.shields.io/badge/NixOS-Declarative-7E7EFF?style=for-the-badge&logo=nixos" alt="NixOS">
  <img src="https://img.shields.io/badge/Windows-Recovery-0078D6?style=for-the-badge&logo=windows" alt="Windows">
  <br>
  <img src="https://img.shields.io/badge/SystemRescue-Stable-orange?style=for-the-badge&logo=linux" alt="SystemRescue">
  <img src="https://img.shields.io/badge/Clonezilla-Disk_Imaging-27ae60?style=for-the-badge&logo=linux" alt="Clonezilla">
  <img src="https://img.shields.io/badge/GParted-Partitioning-orange?style=for-the-badge&logo=linux" alt="GParted">
  <img src="https://img.shields.io/badge/MemTest86+-Hardware-red?style=for-the-badge&logo=linux" alt="MemTest86+">
  <img src="https://img.shields.io/badge/Tails-Privacy-purple?style=for-the-badge&logo=tails" alt="Tails">
</p>

---

## Table of Contents

- [Overview](#overview)
- [Visual Guide](#visual-guide)
- [Toolkit Content](#toolkit-content)
- [Project Structure](#project-structure)
- [Custom Features](#custom-features)
- [Official Links](#official-links)

---

## Overview

Ta clé est un **multiboot toolkit** ultra-complet permettant de démarrer directement des fichiers ISO sans flashage à chaque utilisation. Elle est organisée pour répondre à tous les besoins : installation d'OS, dépannage Windows, forensic, pentesting et maintenance système.

| Category | Tools |
| :--- | :--- |
| **OS** | Arch Linux, Kali Linux, NixOS |
| **Windows / Recovery** | Hiren's BootCD PE |
| **Rescue** | SystemRescue |
| **Disk Management** | Clonezilla, GParted |
| **Hardware Diagnostic** | MemTest86+ |
| **Privacy & Anonymity** | Tails |

---

## Visual Guide

### Boot Menu & OS

| Ventoy Menu | Arch Linux | Kali Linux |
| :---: | :---: | :---: |
| <img src="assets/screenshots/ventoy.png" width="250"> | <img src="assets/screenshots/arch.png" width="250"> | <img src="assets/screenshots/kali.png" width="250"> |

| NixOS | Windows PE | Tails |
| :---: | :---: | :---: |
| <img src="assets/screenshots/nixos.png" width="250"> | <img src="assets/screenshots/windows.png" width="250"> | <img src="assets/screenshots/tails.png" width="250"> |

### Utilities

| GParted | Clonezilla | SystemRescue | MemTest86+ |
| :---: | :---: | :---: | :---: |
| <img src="assets/screenshots/gparted.png" width="180"> | <img src="assets/screenshots/clonezilla.png" width="180"> | <img src="assets/screenshots/rescue.png" width="180"> | <img src="assets/screenshots/memtest.png" width="180"> |

---

## Toolkit Content

### Primary Systems

| | Tool | Description | ISO Filename |
| :---: | :--- | :--- | :--- |
| <img src="assets/arch.png" width="32"> | **Arch Linux** | Minimalist rolling release distribution. | `archlinux-x86_64.iso` |
| <img src="assets/kali.png" width="32"> | **Kali Linux** | Offensive security & pentesting (Persistent). | `kali-linux-live.iso` |
| <img src="assets/nixos.png" width="32"> | **NixOS** | Declarative configuration-based OS. | `nixos-graphical-*.iso` |

### Rescue & Tools

| | Tool | Category | Key Features |
| :---: | :--- | :--- | :--- |
| <img src="assets/windows.png" width="32"> | **Hiren's BootCD PE** | Windows Recovery | Antivirus, Partitioning, Password Reset |
| <img src="assets/rescue.png" width="32"> | **SystemRescue** | Linux Rescue | Boot repair, Filesystem recovery |
| <img src="assets/clonezilla.png" width="32"> | **Clonezilla** | Disk Imaging | Disk cloning and massive deployment |
| <img src="assets/gparted.png" width="32"> | **GParted** | Partitioning | Live partition editor (resize/move/repair) |
| <img src="assets/memtest.png" width="32"> | **MemTest86+** | RAM Diagnostic | Hardware level memory testing |
| <img src="assets/tails.png" width="32"> | **Tails** | Privacy | Amnesic OS with Tor integrated |

---

## Project Structure

```text
/
├── assets/                 # Repository visual assets
│   ├── hero.png            # Hub Hero Image
│   ├── arch.png            # System Logos
│   ├── ...                 # Other Icons
│   └── screenshots/        # Tool & OS Screenshots
├── iso/                    # Main ISO storage
│   ├── ...
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
  Generated by <b>Ventoy Toolkit Manager</b>
</p>
