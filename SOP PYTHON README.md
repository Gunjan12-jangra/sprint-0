# Standard Operating Procedure (SOP's) for Python
---

## Step by Step Installation Guide for Python on Ubuntu
### Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Pre-requisites](#pre-requisites)
4. [Software Overview](#software-overview)
5. [System Requirement](#system-requirement)
6. [Dependencies](#dependencies)
7. [Installation on Ubuntu](#Installation – Ubuntu)
8. [Quick Usage Test](#quick-usage-test)
9. [Troubleshooting](#troubleshooting)
10. [Uninstall Python](#uninstall-python)
11. [Summary](#summary)
12. [Author](#author)
13. [References](#references)
---

## Introduction

Python is a high-level, interpreted programming language widely used for software development, automation, web development, data analysis, artificial intelligence, and more. 
It is designed to be simple, readable, and efficient, making it suitable for beginners and professionals alike. 
Installing Python on Ubuntu ensures that the system can run Python scripts and execute automation tasks effectively.

---

## Features

- Cross-platform: Works on Linux, Windows, and macOS.

- High-level Language: Easy-to-read syntax for quick development.

- Interpreted: No need for compilation, executes code directly.

- Extensive Libraries: Thousands of libraries for various purposes (web, data, AI, networking).

- Community Support: Large active community for troubleshooting and development.

- Open-source: Free to use, modify, and distribute.

---

## Pre-requisites
| Requirement |	Description |
| ---------- | ----------------- |
| User Privileges | sudo privileges required |
| Internet Access	| Required to download Python packages |
| Disk Space |	Minimum 100 MB for Python installation |

---

## Software Overview

| Software	| Version |	Description |
| ------------- | ---------------| ------------------ |
| Python	| 3.x (Recommended 3.11) |	High-level programming language for scripting, automation, and development |

---

## System Requirement
| Parameter	| Minimum Requirement |
| --------- | ---------------- |
| OS |	Ubuntu 20.04 or later |
| RAM |	2 GB |
| Disk Space | 100 MB |
| Internet | Connection	Required |

---

## Dependencies
| Package |	Purpose |
| --------------- | ---------------------------- |
| build-essential |	Required for compiling Python from source |
| libssl-dev |	Secure connections support |
| zlib1g-dev |	Compression library support |
| libncurses5-dev |	Terminal interface support |
| libreadline-dev	| Command-line support |
| libsqlite3-dev |	SQLite database support |
| wget / curl |	Download files and packages |

---

## Installation – Ubuntu 
### Step 1: Update Package 

```bash
sudo apt update -y
```

<img width="1495" height="359" alt="image" src="https://github.com/user-attachments/assets/7c4fe16e-0584-4502-8407-c8af483c228c" />

---

### Step 2: Install Python
#### Option A: Install Default Python Version

```bash
sudo apt install -y python3
```

#### Option B: Install Specific Version (e.g., Python 3.11)

```bash
sudo apt install -y python3.11 python3.11-venv python3.11-dev python3-pip
```

<img width="1359" height="228" alt="image" src="https://github.com/user-attachments/assets/06c69acb-e909-4c46-8acd-84317e2fb147" />

---

### Step 3: Verify Installation

```bash
python3 --version
pip3 --version
```

<img width="1120" height="108" alt="image" src="https://github.com/user-attachments/assets/75c10349-35a8-4428-9298-96d522a25743" />

---

### Step 4: Set Default Python Version (Optional)

```bash
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 1
sudo update-alternatives --config python3
```
---

## Quick Usage Test

#### 1. Open Python REPL:

```bash
python3
```

#### 2. Run a simple test:

```bash
print("Python is installed successfully!")
```

<img width="1313" height="246" alt="image" src="https://github.com/user-attachments/assets/2627be80-2f6d-4780-8bf1-ed1ab00ac7f8" />

---

## Troubleshooting

| Issue |	Solution |
| ----------- | ------------- |
| python3 command not found |	Ensure Python installed: sudo apt install python3 |
| pip not found	| Install pip: sudo apt install python3-pip |
| Permission issues installing packages |	Use: pip3 install --user <package> or sudo pip3 install <package> |

---

## Uninstall Python

```bash
sudo apt remove --purge python3.11 -y
sudo apt autoremove -y
```
---

## Summary

This SOP provides step-by-step instructions to install, verify, and uninstall Python on Ubuntu.

---

## Author

| Name             | Role            | Team                 |
| ---------------- | --------------- | -------------------- |
| Gunjan Jangra | DevOps Trainee | Saarthi |

---

## References
| Links	| Description |
| ------ | ------ |
| https://www.python.org/ | Official Python website |
| https://docs.python.org/3/ | Python documentation |

---
