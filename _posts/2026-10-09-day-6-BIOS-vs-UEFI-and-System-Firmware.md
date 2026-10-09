---
layout: post
title: "Day 6 — BIOS vs. UEFI and System Firmware"
date: 2026-10-9 18:00:00 +0530
categories:
  - Computer Fundamentals
tags:
  - Firmware
  - BIOS
  - UEFI
  - IT Fundamentals
  - Cybersecurity
---

# Day 6 — BIOS vs. UEFI and System Firmware

Today is Day 6 of my learning journal. Yesterday I learned about file systems (NTFS, FAT32, exFAT), file extensions, and basic permissions. Today, I am exploring **Firmware and Boot Interfaces**—specifically **BIOS** and **UEFI**.

Before the operating system loads from the hard drive or SSD, the computer relies on low-level system firmware to test the hardware, configure system settings, and hand off control to the bootloader.

---

## 🎯 What I Want to Learn Today

- What system firmware is and why it runs before the OS
- The main differences between legacy **BIOS** and modern **UEFI**
- The role of **CMOS** and the CMOS battery
- How **Secure Boot** protects systems against early boot malware
- How firmware security connects to cybersecurity and incident response

---

## ⚙️ 1. What is BIOS and UEFI?

Both **BIOS** and **UEFI** are low-level system firmware programs stored on a ROM or Flash memory chip on the motherboard. They perform the initial hardware setup when you press the power button.

### BIOS (Basic Input/Output System)
- **Legacy Interface:** The traditional boot firmware used since the early days of personal computing.
- **Boot Mode:** Uses the **Master Boot Record (MBR)** partitioning scheme, which limits hard drive sizes to 2 TB and a maximum of 4 primary partitions.
- **Interface:** Text-only interface navigated strictly using a keyboard.

### UEFI (Unified Extensible Firmware Interface)
- **Modern Interface:** The successor to traditional BIOS that supports modern hardware architectures.
- **Boot Mode:** Uses the **GUID Partition Table (GPT)** scheme, supporting drives larger than 2 TB (up to 9.4 Zettabytes) and up to 128 primary partitions.
- **Interface:** Graphical user interface (GUI) supporting mouse controls, networking capabilities, and faster boot times.

---

## 🔄 2. Key Differences: BIOS vs. UEFI

| Feature | Legacy BIOS | Modern UEFI |
| :--- | :--- | :--- |
| **Partition Scheme** | Master Boot Record (MBR) | GUID Partition Table (GPT) |
| **Max Drive Size** | **2 TB** | Up to **9.4 Zettabytes** |
| **User Interface** | Text-only (Blue screen / Keyboard) | Graphical UI (Mouse support / Rich menus) |
| **Boot Speed** | Slower (Sequentially initializes hardware) | Fast (Parallel hardware initialization) |
| **Built-in Security** | ❌ None (Vulnerable to MBR rootkits) | ✅ **Secure Boot** (Validates digital signatures) |

---

## 🔋 3. CMOS & The CMOS Battery

- **CMOS (Complementary Metal-Oxide-Semiconductor):** A small onboard memory chip that stores system configuration settings, such as boot device order, hardware parameters, and the system date/time.
- **CMOS Battery (CR2032):** A small coin-cell battery on the motherboard that provides continuous power to the CMOS chip so that time, date, and hardware settings are preserved when the computer is completely unplugged.

---

## 🛡️️ 4. Secure Boot

**Secure Boot** is a critical security feature built into UEFI firmware:

1. **Digital Signature Check:** When the computer boots, UEFI verifies the cryptographic signature of the bootloader software (e.g., Windows Boot Manager or GRUB).
2. **Execution Gate:** If the bootloader signature is valid and trusted by the hardware manufacturer, the OS kernel is allowed to boot.
3. **Malware Prevention:** If a rootkit or bootkit has tampered with the boot files, the signature check fails, preventing the malicious code from executing.

---

## 🧠 Connection to Cybersecurity

- **Rootkits & Bootkits:** Malicious software that targets the MBR or UEFI firmware loads *before* the operating system or antivirus software initializes, making detection difficult.
- **Firmware Updates:** Keeping UEFI firmware updated patched known hardware-level vulnerabilities and prevents unauthorized flashing.
- **CMOS Reset Attacks:** Disconnecting the CMOS battery on older hardware can reset administrative firmware passwords, posing physical security considerations.

---

## 📝 What I Learned Today

- **BIOS** is the legacy text-based firmware limited by 2 TB drives (MBR), while **UEFI** is the modern GUI replacement supporting GPT partitions over 2 TB.
- The **CMOS Battery** supplies continuous power to hold BIOS/UEFI settings and real-time clock data when power is disconnected.
- **Secure Boot** uses digital certificates in UEFI to stop unauthorized bootloaders and rootkits from starting up.

---

## 🤔 My Reflection

Learning about UEFI and Secure Boot helped me realize that operating system security begins long before Windows or Linux boots up. Protecting the boot process at the hardware level ensures that the integrity of the operating system remains uncompromised right from the moment power is applied.

---

## 🚀 What's Next?

In my next lesson, I will learn about:

11. **Computer Ports & Connectors**
    - USB
    - HDMI
    - Ethernet
    - DisplayPort
    - Audio ports

> **One concept. One lab. One lesson at a time.**
