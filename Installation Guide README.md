# Python Installation Guide - Documentation

---

## Authors

| Author           | Created    | Version | Last updated by  | Last Edited On | Pre Reviewer | L0 Reviewer | L1 Reviewer | L2 Reviewer |
| ---------------- |---------------- | ------- | ---------------- | -------------- | ------------ | ----------- | ----------- | ----------- |
| Gunjan Jangra  |  22-01-2026    |  1.0     | Gunjan Jangra |  22-01-2026     |              |             |             |             |

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [Why Python](#2-why-python)
3. [Installation on Ubuntu](#3-installation-on-ubuntu)
4. [Quick Usage Test](#4-quick-usage-test)
5. [Troubleshooting](#5-troubleshooting)
6. [Contact Information](#6-contact-information)
7. [References](#7-references)
8. [End Note](#8-end-note)

---

## 1. Introduction

Python is a high-level, interpreted programming language widely used for software development, automation, web development, data analysis, artificial intelligence, and more. 
It is designed to be simple, readable, and efficient, making it suitable for beginners and professionals alike. 

---

## 2. Why Python?

Python is widely used because:

- It is cross-platform (Linux, Windows, macOS).

- It simplifies automation in DevOps, cloud, and scripting workflows.

- Supports libraries for AI, data analysis, web development, and networking.

- Reduces complexity in scripts and pipelines.

- Integrates with Docker, Terraform, Jenkins and Ansible

---

## 3. Installation on Ubuntu
### Step 1: Update Package 

```bash
sudo apt update -y
```
---

### Step 2: Install Python
#### Option A: Install Default Python Version

```bash
sudo apt install -y python3
sudo apt install -y python3-pip
```
---

#### Option B: Install Specific Version (e.g., Python 3.11)

```bash
sudo apt install -y python3.11 python3.11-venv python3.11-dev python3-pip
```
---

### Step 3: Verify Installation

```bash
python3 --version
pip3 --version
```
---

### Step 4: Set Default Python Version (Optional)

If multiple versions are installed:

```bash
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 1
sudo update-alternatives --config python3
```
---

## 4. Quick Usage Test

#### 1. Open Python REPL:

```bash
python3
```

#### 2. Run a simple test:

```bash
print("Python is installed successfully!")
```
---

## 5. Troubleshooting
| Issue |	Solution |
| ------ | ------- |
| python3 command not found |	Install Python: sudo apt install python3 |
| pip not found	 | Install pip: sudo apt install python3-pip |
| Permission issues installing packages |	Use: pip3 install --user <package> or sudo pip3 install <package> |

---

## 6. Contact Information

| Contact Type | Details                                                             |
| ------------ | ------------------------------------------------------------------- |
| Email        | [jangragunjan39@gmail.com](mailto:jangragunjan39@gmail.com) |

---

## 7. References
| Links	| Description |
| ------ | ------ |
| https://www.python.org/ | Official Python website |
| https://docs.python.org/3/ | Python documentation |

---

## 8. End Note

This documentation provides a step-by-step guide for installing, verifying, and using Python on Ubuntu.

---
