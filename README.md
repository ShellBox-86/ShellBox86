<p align="center">
  <img src="https://i.ibb.co/rfZFZhf8/New-Project-1.png" alt="ShellBox86 logo" width="128">
</p>

<h1 align="center">ShellBox86 Operating System</h1>
<p align="center">A lightweight legacy x86 OS that fits on a single floppy</p>

## 🧠 About

**ShellBox86** is a simple, educational operating system designed for legacy x86 machines.  
Its entire core — including the bootloader, kernel, and basic system functionality — fits within a single **1.44MB floppy disk image**.

It is built from scratch using Assembly and C, and is ideal for low-level system development, experimentation, or retro hardware projects.

## 🎯 Scope

- 🖥️ Runs on real-mode BIOS x86 hardware (no UEFI)
- 💾 Boots entirely from a 1.44MB floppy disk
- 🔧 Includes a custom bootloader, kernel, and basic shell
- 💡 Built for simplicity, speed, and minimalism
- 🧪 Suitable for vintage hardware in case you want to run *modern* (not really) software

## ⚙️ Getting Started

### Prerequisites

- `nasm` – assembler
- `gcc` – cross-compiler (or system compiler with freestanding options)
- `qemu` or `bochs` – emulator for testing

### Build & Run

```bash
make floppy.img
qemu-system-i386 -fda floppy.img
```

> 💡 You can also write the image to a real floppy disk using `dd`.

## 📜 License

This project is licensed under the **BSD 2-Clause License**.  
See the [`LICENSE`](./LICENSE) file for details.

<p align="center"><em>Built with 💖 and 💾 by the ShellBox86 team</em></p>
