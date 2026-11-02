# 🧪 Project: ZunkerBot Deconstruction & Analysis Lab

![Research Status](https://shields.io)
![Environment](https://shields.io)
![Code Quality](https://shields.io)

A historical analysis and defensive engineering lab focused on dissecting **ZunkerBot** (a legacy 2007-era web-based botnet control infrastructure). This repository is dedicated purely to threat intelligence, signature generation, and understanding legacy command-and-control (C2) architecture.

---

## 🛑 Critical Safety Disclaimer

> [!CAUTION]
> **WARNING:** The contents of this repository involve legacy malware components. 
> * **DO NOT** execute any binaries outside a strictly isolated, host-only sandbox or air-gapped virtual machine.
> * This project is maintained exclusively for academic research, reverse engineering education, and indicators of compromise (IoC) extraction.

---

## 🏗️ Architecture Overview

The ZunkerBot ecosystem consists of two primary architectural components:

* 💻 **Client Agent (Bot):** Compiled binary components originally authored in **Delphi / C++** designed to receive instructions for spam execution.
* 🌐 **Control Panel (C2 Server):** A web-based administration panel written in **PHP** utilizing a **MySQL** backend to track active nodes and queue tasks.

---

## 📁 Repository Structure

```text
├── c2-panel/          # Deconstructed PHP administrative panel source files
│   ├── assets/        # Panel styles and interface layouts
│   └── database/      # SQL structure definitions and historical schemas
├── client-src/        # Decompiled or reverse-engineered agent stubs (Delphi/C++)
├── signatures/        # Extracted YARA rules and network IoCs
├── .gitignore         # Strict exclusion rules for local builds and configs
└── README.md          # Project documentation
```

---

## 🛠️ Lab Setup Guidelines

To safely review the control panel structure or test database query behaviors in a local, non-routing environment:

### 1. Environment Requirements
* 📦 **Virtualization:** VMware Workstation or VirtualBox configured with **Host-Only networking**.
* 🛡️ **Web Server:** A local LAMP/WAMP stack (PHP 5.6 legacy compatibility may be required due to the age of the codebase).

### 2. Initialization Steps
1. Clone this repository into your isolated analysis environment.
2. Copy `config.php.example` to `config.php` and fill in local database loopback credentials.
3. Import the safe structural schema from `/c2-panel/database/schema.sql` to inspect database relational tables.

---

## 🔍 Analytical Objectives

* [ ] **Database Relational Mapping:** Document how the panel tracks unique hardware IDs.
* [ ] **Network Protocol Analysis:** Reconstruct the precise HTTP POST/GET request formats expected by the C2 listeners.
* [ ] **YARA Development:** Author localized YARA rules to detect legacy string fragments associated with the agent installer.
