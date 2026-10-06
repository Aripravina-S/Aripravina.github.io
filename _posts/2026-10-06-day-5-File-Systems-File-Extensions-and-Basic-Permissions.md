---
layout: post
title: "Day 5 — File Systems, File Extensions, and Basic Permissions"
date: 2026-10-06 17:58:00 +0530
categories:
  - Computer Fundamentals
tags:
  - File Systems
  - NTFS
  - FAT32
  - exFAT
  - IT Fundamentals
  - Cybersecurity
---

# Day 5 — File Systems, File Extensions, and Basic Permissions

Today is Day 5 of my learning journal. Yesterday I learned about software classifications, memory types, and the storage hierarchy. Today, I am diving into **File Systems**—how operating systems organize, store, name, and protect files on hard drives and flash memory.

Understanding file systems helps clarify how files are structured, how permissions protect sensitive data, and why choosing the right file system matters for compatibility and security.

---

## 🎯 What I Want to Learn Today

- What Files & Folders are and how directory trees organize data
- Why File Extensions are important (and how attackers exploit them)
- The main file systems: **NTFS**, **FAT32**, and **exFAT**
- Basic File Permissions (Read, Write, Execute)
- How file system features connect to cybersecurity

---

## 📁 1. Files & Folders

At the most basic level, all data on a drive is stored as files and organized using folders:

- **File:** A collection of related data stored under a single name (e.g., text, image, executable program).
- **Folder (Directory):** A container used to group and organize files into a hierarchical tree structure.

---

## 📄 2. File Extensions

A **File Extension** is the suffix at the end of a filename (after the dot `.`) that tells the operating system which program should open the file.

| Extension | Category | Example Use |
| :--- | :--- | :--- |
| `.txt`, `.docx`, `.pdf` | Documents | Text files, word processor documents, PDFs |
| `.jpg`, `.png`, `.gif` | Images | Compressed photos, transparent graphics, animations |
| `.exe`, `.bat`, `.sh` | Executables | Executable binaries, Windows batch scripts, Linux shell scripts |
| `.zip`, `.tar.gz` | Archives | Compressed folders containing multiple files |

> ⚠️ **Security Warning:** Attackers often try to hide malicious executable files by using double extensions (e.g., `invoice.pdf.exe`). If file extensions are hidden in Windows Explorer, a user might mistake it for a safe PDF document.

---

## 💾 3. File Systems Compared (NTFS vs. FAT32 vs. exFAT)

A **File System** is the internal method and data structure an operating system uses to control how data is stored and retrieved on a disk partition.

| Feature | FAT32 | exFAT | NTFS |
| :--- | :--- | :--- | :--- |
| **Full Name** | File Allocation Table 32 | Extended File Allocation Table | New Technology File System |
| **Max File Size** | **4 GB** (Cannot store files larger than 4GB) | 16 EB (Exabytes - virtually unlimited) | 8 PB (Petabytes) |
| **Compatibility** | Universal (Windows, Mac, Linux, TV, Consoles) | Broad (Windows, Mac, Android, Cameras) | Primary for Windows (Read-only on Mac by default) |
| **File Permissions** | ❌ No native security permissions | ❌ No native security permissions | ✅ Full Access Control Lists (ACLs) |
| **Encryption/Journaling** | ❌ None | ❌ None | ✅ EFS Encryption & Journaling (prevents corruption) |
| **Best Used For** | Small USB flash drives, legacy hardware | SD cards, external cross-platform drives | Windows primary boot drive (C:) |

---

## 🔒 4. Basic File Permissions

Permissions determine **who** can interact with a file or folder and **what** actions they can perform.

### Standard Permissions:
1. **Read (r):** Allows viewing or opening the file contents / listing folder items.
2. **Write (w):** Allows modifying, editing, renaming, or deleting the file or folder.
3. **Execute (x):** Allows running a file as a script or program / traversing a folder.


- **Access Control Lists (ACLs):** On NTFS file systems, fine-grained rules specify exactly which user accounts or group accounts have access rights.

---

## 🧠 Connection to Cybersecurity

- **NTFS Journaling & Forensics:** NTFS keeps a log (Journal) of file changes, helping digital forensics investigators recover deleted files and track timestamps.
- **Malicious File Execution:** Attackers upload `.php` or `.exe` files disguised as images (`avatar.jpg.exe`) to bypass basic file upload filters on servers.
- **Privilege Escalation:** Weak file permissions on system directories allow low-privilege users to modify executable files run by system administrators or services.

---

## 📝 What I Learned Today

- **File Extensions** instruct the OS on how to open a file, but can be spoofed by attackers.
- **FAT32** is highly compatible but limited by a 4 GB max file size and lacks file permissions.
- **exFAT** is ideal for large USB drives used across Windows and macOS.
- **NTFS** is the modern Windows default that supports large files, journaling, encryption, and granular security permissions.
- **Basic Permissions (Read, Write, Execute)** prevent unauthorized users from editing or running critical system files.

---

## 🤔 My Reflection

Learning about file system features made me realize why Windows uses NTFS for system drives while camera SD cards use exFAT. Security features like permissions and encryption rely directly on the file system underneath—without NTFS, Windows wouldn't be able to restrict unauthorized users from reading system files.

---

## 🚀 What's Next?

In my next lesson, I will learn about:

- BIOS & UEFI

> **One concept. One lab. One lesson at a time.**
