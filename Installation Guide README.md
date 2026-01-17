# Python Installation Guide
---

## Document Details
| Author | Created on | Last updated by |	Last edited on |
|-------- | ---------| -------- | -------- |
| Gunjan |	18-01-2026 |	Gunjan |	18-01-2026 |

---

## Index

1. Introduction
2. Why Python?
3. Installation on Ubuntu
4. Quick Usage Test
5. Troubleshooting
6. References
7. End Note

---

## Introduction

Python is a high-level, interpreted programming language widely used for software development, automation, web development, data analysis, artificial intelligence, and more. 
It is designed to be simple, readable, and efficient, making it suitable for beginners and professionals alike. 
Installing Python on Ubuntu ensures that the system can run Python scripts and execute automation tasks effectively.
This documentation explains how to install, verify, and use Python on Ubuntu.

---

## Why Python?

Python is widely used because:

- It is cross-platform (Linux, Windows, macOS).

- It simplifies automation in DevOps, cloud, and scripting workflows.

- Supports libraries for AI, data analysis, web development, and networking.

- Reduces complexity in scripts and pipelines.

- Integrates with Docker, Terraform, Jenkins and Ansible

---

## Installation on Ubuntu
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

## Quick Usage Test

#### 1. Open Python REPL:

```bash
python3
```

#### 2. Run a simple test:

```bash
print("Python is installed successfully!")
```
---

## Troubleshooting
| Issue |	Solution |
| ------ | ------- |
| python3 command not found |	Install Python: sudo apt install python3 |
| pip not found	 | Install pip: sudo apt install python3-pip |
| Permission issues installing packages |	Use: pip3 install --user <package> or sudo pip3 install <package> |

---

## References
| Links	| Description |
| ------ | ------ |
| https://www.python.org/ | Official Python website |
| https://docs.python.org/3/ | Python documentation |

---

## End Note

This documentation provides a step-by-step guide for installing, verifying, and using Python on Ubuntu.

---
