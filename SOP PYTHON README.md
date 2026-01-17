# Standard Operating Procedure (SOP's) for Python
---

## Step by Step Installation Guide for Python on Ubuntu
### Table of Contents

1. Introduction

2. Features

3. Purpose

4. Pre-requisites

5. Software Overview

6. System Requirement

7. Dependencies

8. Installation on Ubuntu 

9. Quick Usage Test

10. Troubleshooting

11. Uninstall Python

12. Examples

13. Summary

14. Author

15. References

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

## System Requirement
| Parameter	| Minimum Requirement |
| --------- | ---------------- |
| OS |	Ubuntu 20.04 or later |
| RAM |	2 GB |
| Disk Space | 100 MB |
| Internet | Connection	Required |

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

## Installation – Ubuntu 
Step 1: Update Package Index
sudo apt update -y


Step 2: Install Python
Option A: Install Default Python Version
sudo apt install -y python3

Option B: Install Specific Version (e.g., Python 3.11)
sudo apt install -y python3.11 python3.11-venv python3.11-dev python3-pip

Step 3: Verify Installation
python3 --version
pip3 --version


Expected Output: Python 3.x.x and pip x.x.x

Step 4: Set Default Python Version (Optional)
sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.11 1
sudo update-alternatives --config python3

9. Quick Usage Test

Open Python REPL:

python3


Run a simple test:

print("Python is installed successfully!")

10. Troubleshooting
Issue	Solution
python3 command not found	Ensure Python installed: sudo apt install python3
pip not found	Install pip: sudo apt install python3-pip
Permission issues installing packages	Use: pip3 install --user <package> or sudo pip3 install <package>
11. Uninstall Python
sudo apt remove --purge python3.11 -y
sudo apt autoremove -y


Verify removal:

python3 --version
