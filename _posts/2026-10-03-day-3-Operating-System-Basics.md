---
layout: post
title: "Day 3 — Operating System Basics"
date: 2026-10-03 17:43:00 +0530
categories:
  - Computer Fundamentals
tags:
  - Operating Systems
  - Linux
  - Windows
  - IT Fundamentals
  - Cybersecurity
---

# Day 3 — Operating System Basics

Today is Day 3 of my learning journal. Yesterday I learned about hardware parts like the CPU and RAM. Today, I am learning about **Operating System (OS) Basics**—the software that controls all that hardware and brings the computer to life.

I used to think an OS was just a desktop screen where I open apps. Today I learned what happens behind the screen to manage processes, memory, and startup steps.

---

## 🎯 What I Want to Learn Today

- What an Operating System (OS) actually does
- The difference between the Kernel and the Shell
- What a Process and a Thread are
- The step-by-step Boot Process
- The difference between Multitasking and Multiprocessing
- How OS concepts relate to cybersecurity

---

## 🖥️ Operating System (OS) & Functions

An **Operating System (OS)** is the main system software that sits between computer hardware and the user. Without an OS, you would have to write complex code just to tell the computer to show a letter on the monitor or save a file.

### Main Functions of an OS:
1. **Process Management:** Decides which program gets to run on the CPU and for how long.
2. **Memory Management:** Allocates RAM space to apps when they open and cleans it up when they close.
3. **File System Management:** Organizes files, folders, and permissions on the SSD or Hard Disk.
4. **Device Management:** Uses special software drivers to communicate with printers, keyboards, and network cards.
5. **Security & Access Control:** Uses user passwords, privileges, and permissions to protect system files.

---

## 🧠 Kernel vs. Shell

An Operating System has two main layers that work together:

### 1. Kernel (The Core)
The **Kernel** is the heart of the operating system. It runs continuously in a protected area of memory and has complete control over everything in the system. It directly instructs the CPU, RAM, and hardware devices on what to do.

### 2. Shell (The Interface)
The **Shell** is the outer layer that takes input commands from the user and translates them into instructions the Kernel understands.
- **GUI (Graphical Shell):** Clicking icons and windows with a mouse (like Windows Explorer).
- **CLI (Command-Line Shell):** Typing text commands into a terminal (like Bash in Linux or PowerShell in Windows).

---

## ⚙️ Process vs. Thread

### 1. Process
A **Process** is a program that is currently running in memory. When you open an application like a web browser, the OS loads its files into RAM and assigns it a unique identifier called a **Process ID (PID)**.

### 2. Thread
A **Thread** is a single path of execution inside a process. Think of a process as a whole workplace and a thread as an individual worker inside it. 

> **Example:** In a web browser (the Process), one Thread displays the webpage, another Thread downloads a file, and a third Thread handles audio playback.

---

## 🔄 Boot Process (How a Computer Turns On)

When you press the power button on a computer, it goes through a standard sequence of steps before showing your desktop:

1. **Power Supply Check:** Power reaches the motherboard and components.
2. **POST (Power-On Self-Test):** The BIOS/UEFI checks hardware (RAM, keyboard, drive) to ensure everything is functioning.
3. **Bootloader Execution:** The system locates the boot drive and loads the **Bootloader** program (like Windows Boot Manager or Linux GRUB).
4. **Kernel Loading:** The bootloader loads the OS **Kernel** into RAM.
5. **System Services & Login:** The kernel initializes background drivers and starts the user login screen.

---

## 🔀 Multitasking vs. Multiprocessing

| Feature | Multitasking | Multiprocessing |
| :--- | :--- | :--- |
| **Concept** | Running multiple tasks/apps seemingly at the same time by quickly switching between them. | Using **two or more physical CPUs/cores** to run multiple instructions simultaneously. |
| **Hardware** | Can be done on a single CPU core. | Requires multiple CPU cores or CPUs. |
| **Example** | Listening to music while typing a document on one core. | Rendering a video on Core 1 while scanning for viruses on Core 2. |

---

## 🧠 Connection to Cybersecurity

- **Process Monitoring (PIDs):** Security analysts monitor running processes (using Task Manager or `ps` in Linux) to detect unauthorized tools or malware executing in memory.
- **Kernel-Level Attacks:** Attackers try to exploit system vulnerabilities to elevate their permissions from regular user space up into the **Kernel**, gaining total control of the system.
- **Boot Integrity:** Security mechanisms like **Secure Boot** prevent malicious rootkits from infecting the bootloader during system startup.

---

## 📝 What I Learned Today

- The **Kernel** manages hardware directly, while the **Shell** takes user commands.
- A **Process** is an active program in RAM with a PID, and a **Thread** is a smaller unit of execution inside that process.
- The **Boot Process** moves from hardware checks (POST) to the bootloader, kernel initialization, and final user login screen.
- **Multitasking** switches between tasks quickly on one core, while **Multiprocessing** runs tasks at the same time on separate CPU cores.

---

## 🤔 My Reflection

Learning how the OS coordinates memory and processes makes command-line interfaces feel much clearer. When I look at running background services or terminal outputs, I now understand that every action corresponds to a specific process running under kernel supervision.

---

## 🚀 What's Next?

In my next lesson, I will learn about:

**Software**
   - System Software
   - Application Software
   - Utility Software
   - Firmware
   - Open Source vs Proprietary
     
**Memory & Storage**
   - Primary Memory
   - Secondary Memory
   - Virtual Memory

> **One concept. One lab. One lesson at a time.**
