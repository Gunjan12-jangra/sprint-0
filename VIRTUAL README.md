# Standard Operating Procedure (SOP's) for Python Virtual Environment
## Managing Python Virtual Environment (venv) on Ubuntu
---

## Table of Contents

1. Introduction
2. Features
3. Purpose
4. Pre-requisites
5. Software Overview
6. System Requirement
7. Dependencies
8. Virtual Environment Management (with Examples)
9. Troubleshooting
10. Summary
11. Author
12. References

---

## Introduction

Python Virtual Environment (venv) is a tool that helps create an isolated Python environment for a specific project.
It allows users to install and manage project-specific Python packages without affecting the system-wide Python installation.
This is especially useful when working on multiple projects that require different package versions.

---

## Features

Python Virtual Environment provides the following features:

- Isolates project dependencies
- Prevents package version conflicts
- Keeps system Python clean
- Allows easy dependency management
- Helps recreate environments using requirements files
- Beginner-friendly and lightweight

---

## Purpose

Python virtual environments are used to:

- Manage project-specific Python packages
- Avoid dependency conflicts between projects
- Improve application stability
- Support clean development practices
- Simplify Python project setup for beginners
- 
---

## Pre-requisites

| Requirement |	Description |
| ----------- | -------------------- |
| OS Access |	User must have access to Linux system |
| Python |	Python 3 must be installed |
| Privileges |	Normal user access (sudo not recommended for pip) |

---

## Software Overview

| Software |	Description |
| ------------ | ------------|
| Python |	Programming language |
| venv |	Built-in Python module for virtual environments |
| pip	| Python package manager |

---

## System Requirement

| Requirement |	Minimum Recommendation |
| -------------- | ---------------------- |
| OS | 	Ubuntu |
| Python | Version	Python 3.x |
| RAM	 | 1 GB or higher |
| Disk |	100 MB or higher |

---

## Dependencies
| Dependency | Description |
| ---------------- | ---------------------------------- |
| python3-venv | Package required to create virtual environments |

➡️ Note: Most modern Ubuntu versions come with venv support by default.

---

## Virtual Environment Management using venv
### 1. Create a Virtual Environment

Used to create a new isolated Python environment.

#### Syntax:

```bash
python3 -m venv <env-name>
```

#### Example:

```bash
python3 -m venv myenv
```
---

### 2. Activate a Virtual Environment

Used to activate the virtual environment.

#### Syntax:

```bash
source <env-name>/bin/activate
```

#### Example:

```bash
source myenv/bin/activate
```

Once activated, the environment name appears in the terminal prompt.

---

### 3. Install Packages

Used to install Python packages inside the virtual environment.

#### Syntax:

```bash
pip install <package-name>
```

#### Example:

```bash
pip install flask
```

<img width="1856" height="580" alt="image" src="https://github.com/user-attachments/assets/b935a19f-71e1-4604-afd3-cb49a4ccfd0c" />

---

### 4. Freeze Installed Packages

Used to save installed dependencies into a file.

#### Syntax:

```bash
pip freeze > requirements.txt
```

#### Example:

```bash
pip freeze > requirements.txt
```

---

### 5. Deactivate a Virtual Environment

Used to exit the virtual environment.

#### Syntax:

```bash
deactivate
```
---

### 6. Delete a Virtual Environment

Used to permanently remove the virtual environment.

#### Syntax:

```bash
rm -rf <env-name>
```

#### Example:

```bash
rm -rf myenv
```

<img width="1693" height="314" alt="image" src="https://github.com/user-attachments/assets/2286ac3f-e6e6-46da-81c3-dcdaf43288af" />

---

## Troubleshooting
### Activation Error

- Ensure correct directory path

```bash
ls myenv/bin/activate
```

### Permission Problems

- Avoid using sudo with pip

```bash
chmod -R u+rwx myenv
```

### pip Not Found

```bash
python3 -m ensurepip --default-pip
```
---

## Summary

Python Virtual Environments are essential for managing dependencies in Python projects.
They provide isolation, prevent conflicts, and ensure consistent development environments, making them ideal for both beginners and professionals.

---

## Author
| Name |	Role |	Team |
|----------- | ------------ | ---------------- |
| Gunjan Jangra	| DevOps Trainee |	Saarthi |

---

## References
| Reference |	Link |
| ------------------------------ | ----------------------------- |
| Python Official Documentation – venv |	https://docs.python.org/3/library/venv.html |
| Python Packaging Guide |	https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/ |

---
