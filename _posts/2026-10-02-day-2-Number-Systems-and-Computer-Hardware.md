---
layout: post
title: "Day 2 — Number Systems and Computer Hardware"
date: 2026-10-02 17:10:00 +0530
categories:
  - Computer Fundamentals
tags:
  - Hardware
  - Number Systems
  - IT Fundamentals
  - Cybersecurity
---

# Day 2 — Number Systems and Computer Hardware

Today is Day 2 of my learning journal. Yesterday I looked at what a computer is. Today, I am learning two basic topics: **Number Systems** and **Computer Hardware**.

I used to wonder why computers use numbers like `0` and `1` or letters like `A` and `F`. Today I learned why they are used and what the basic parts inside a computer do.

---

## 🎯 What I Want to Learn Today

- The 4 basic number systems in computers
- Why Binary and Hexadecimal are important
- The main physical parts inside a computer
- The difference between temporary memory and permanent storage
- How all of this relates to cybersecurity

---

## 🔢 Number Systems

Computers do not understand English. They only work with electricity—either **ON** or **OFF**. To understand this, we use four different number systems:

### 1. Decimal (Base-10)
This is the normal counting system we use every day: `0, 1, 2, 3, 4, 5, 6, 7, 8, 9`.

### 2. Binary (Base-2)
This is the computer's own language. It only uses two numbers: `0` (OFF) and `1` (ON). Each `0` or `1` is called a **bit**.

### 3. Octal (Base-8)
Uses numbers from `0` to `7`. It is used in Linux to set file permissions (like `755`).

### 4. Hexadecimal (Base-16)
Uses numbers `0` to `9` and letters `A` to `F` (where A=10 and F=15). 

Binary numbers get super long (like `11111111`). Hexadecimal is just a shorter, easier way for humans to read long binary numbers.

| Decimal | Binary | Octal | Hexadecimal |
| :--- | :--- | :--- | :--- |
| **0** | `0000` | `0` | `0` |
| **5** | `0101` | `5` | `5` |
| **10** | `1010` | `12` | `A` |
| **15** | `1111` | `17` | `F` |
| **255** | `11111111` | `377` | `FF` |

---

## 🛠️ Basic Computer Hardware

Hardware means the physical parts of a computer that you can see and touch.

### 1. CPU (Central Processing Unit)
The "brain" of the computer. It calculates data and runs all commands.

### 2. Motherboard
The big main board inside the computer that connects all parts (CPU, RAM, hard disk) together.

### 3. RAM (Random Access Memory)
The computer's **short-term memory**. When you open an app, it loads into RAM. When you turn off the computer, everything in RAM disappears.

### 4. ROM (Read-Only Memory)
Permanent memory that holds startup instructions (BIOS) so the computer knows how to turn on.

### 5. Cache Memory
A tiny, super-fast memory right inside the CPU used to hold things the CPU needs repeatedly.

### 6. HDD (Hard Disk Drive)
An older, larger storage device that uses a spinning disk to save files permanently.

### 7. SSD (Solid-State Drive)
Newer, faster storage with no moving parts. It works like a big USB drive and loads files much quicker than an HDD.

### 8. SMPS (Power Supply)
Converts electricity from the wall socket into safe power for the internal computer parts.

### 9. GPU (Graphics Card)
A special chip built to handle display graphics, videos, and games.

### 10. NIC (Network Card)
The chip or card that lets your computer connect to Wi-Fi or an Ethernet cable. It has a unique physical address called a **MAC Address**.

### 11. Input & Output Devices
- **Input:** Keyboard, mouse (you send data IN).
- **Output:** Monitor, speaker (computer sends data OUT).

---

## 🧠 Connection to Cybersecurity

- **Hexadecimal in Security:** Computer addresses (like MAC addresses) and secret codes in files are written in Hexadecimal.
- **RAM Investigation:** Sometimes attackers run malicious scripts in temporary memory (RAM). Security analysts inspect RAM to find what the attacker was doing.
- **Network Cards (NIC):** Checking MAC addresses helps security teams identify unknown devices connected to a network.

---

## 📝 What I Learned Today

- Computers speak **Binary** (`0` and `1`), but we use **Hexadecimal** to read it easily.
- **RAM** is temporary short-term memory; **HDD/SSD** is permanent storage.
- The **CPU** is the brain, and the **Motherboard** connects every part together.
- Understanding hardware helps me know where files and logs are kept during a security investigation.

---

## 🤔 My Reflection

Today helped me realize that numbers like `0x41` or MAC addresses are not random secrets—they are just simple Hexadecimal numbers that represent real data stored inside RAM or files. Knowing where data lives makes it much easier to learn how to defend computers.

---

## 🚀 What's Next?

In my next lesson, I will learn about:

- What an Operating System (OS) does
- Basic difference between Windows and Linux
- What a process is
- Simple file systems

> **One concept. One lab. One lesson at a time.**
