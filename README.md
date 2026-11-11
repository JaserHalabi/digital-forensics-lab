# Digital Forensics Lab

[![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue?style=flat-square)](https://www.kali.org)
[![Discipline](https://img.shields.io/badge/Focus-Digital%20Forensics%20%26%20Incident%20Response-informational?style=flat-square)](#overview)
[![Status](https://img.shields.io/badge/Labs%20Completed-1%20Verified-success?style=flat-square)](#lab-execution-matrix)
[![Engineer](https://img.shields.io/badge/Investigator-Jaser%20Halabi-lightgrey?style=flat-square&logo=github)](https://github.com/JaserHalabi)

> A practical portfolio of digital forensics investigations, covering evidence analysis, artifact recovery, steganography, password cracking and chain-of-custody verification, carried out with open-source forensic tooling on **Kali Linux**.

---

## Overview

This repository documents hands-on forensic investigations. Each lab is a full case: real evidence files examined with industry-standard tools, step-by-step analysis backed by screenshots, and a final reconstruction of what happened and how to defend against it.

### Core Forensic Competencies

- **Metadata & Artifact Analysis:** EXIF inspection, hidden comments, device fingerprinting and GPS geolocation.
- **File Carving:** Detecting and extracting embedded or appended files from carrier media.
- **Password Recovery:** Hash extraction and dictionary attacks against protected archives.
- **Steganography & Steganalysis:** Recovering payloads hidden inside images.
- **Image Forensics:** Enhancing photos to recover detail that isn't visible to the eye.
- **Evidence Integrity:** Hash-based verification to preserve chain of custody.
- **Attack Reconstruction:** Mapping attacker techniques to MITRE ATT&CK and recommending defenses.

---

## Featured Investigations

| Investigation | Forensic Focus | Key Tools | Verification Capture |
|---|---|---|---|
| **[Steganography & Data Leak Investigation](./Steganography-Data-Leak-Investigation/)** | Insider leak hidden in a photo across 3 layers: appended ZIP, password protection and steganography | `exiftool`, `binwalk`, `zip2john`, `john`, `steghide`, Forensically | [Recovered Leak & Flag](./Steganography-Data-Leak-Investigation/leak-flag.png) |

---

## Lab Execution Matrix

| # | Lab Module | Forensic Focus | Status | Completed |
|---|---|---|:---:|:---:|
| 01 | [Steganography & Data Leak Investigation](./Steganography-Data-Leak-Investigation/) | EXIF analysis, file carving, ZIP cracking, image enhancement, Steghide extraction and SHA-256 verification | Complete | 2026-11-11 |

> *More investigations will be documented and published here as they are completed.*

---

## Environment & Tooling

- **Forensic Workstation:** Kali Linux (VM)
- **Metadata Analysis:** ExifTool
- **File Carving:** Binwalk
- **Password Recovery:** John the Ripper (`zip2john`)
- **Steganography:** Steghide
- **Image Forensics:** [Forensically](https://29a.ch/photo-forensics/)
- **Integrity Verification:** SHA-1 / SHA-256 hashing

---

_Maintained by **[Jaser Halabi](https://github.com/JaserHalabi)**_
