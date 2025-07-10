# Disk Image Acquisition & Hash Verification

This repository contains a digital forensic report documenting the acquisition and integrity verification process of a disk image from a virtual machine named `DionaeaHoneypot`.

## 📌 Project Overview

The purpose of this task was to ensure that the `.vdi` disk image acquired from the honeypot environment was an exact and untampered copy of the original disk. The process followed standard forensic procedures, including cryptographic hash generation using both **MD5** and **SHA-256** algorithms.

## 🧪 Tools Used

- **Windows PowerShell** – for generating file hash values.
- **Manual Acquisition** – copying the `.vdi` file from the host system.

## 🧾 Evidence Details

| Item              | Description                                     |
|-------------------|-------------------------------------------------|
| Virtual Machine   | DionaeaHoneypot                                 |
| Disk Format       | `.vdi` (VirtualBox Disk Image)                  |
| Original Size     | 35.00 GB (virtual size)                         |
| Actual File Size  | 4.76 GB                                         |
| Storage Path      | `D:\evidence\DionaeaHoneypot\`                  |
| Acquisition Date  | July 2, 2025                                    |

## 🔐 Hash Verification

| Algorithm | Hash Value                                                                 |
|-----------|-----------------------------------------------------------------------------|
| **MD5**   | `56BCD3F56F1B7395C4BE717C9A56EC0D`                                          |
| **SHA256**| `ABE58454E1E76FD25FCAD6B71E996505756F5F1E211A26FBFEC03C22ED9256B5`         |

These values were generated immediately after acquisition and confirmed to remain unchanged, validating the integrity of the disk image.

## 📜 Chain of Custody

| Date & Time      | Person         | Action                     | Location                  |
|------------------|----------------|----------------------------|---------------------------|
| 2025-07-02 21:55 | Marco Albert   | Copied `.vdi` from VM      | `D:\evidence\...`         |
| 2025-07-02 22:15 | Marco Albert   | Generated hash values      | `D:\evidence`             |

## ✅ Conclusion

The acquisition and verification process was successful. The integrity of the virtual disk image was preserved, ensuring it can be used as admissible digital evidence in forensic investigations.

---

**Prepared by:**  
**Marco Albert**  
**Internship Role:** Digital Forensics & Investigator  
**Institution:** [Cyborts]  
**Date:** July 2, 2025
