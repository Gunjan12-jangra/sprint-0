# Python Virtual Environments

Why, how to setup, best practices

---

## 📌 Table of Contents
1. [Author Information](#1-author-information)
2. [Introduction](#2-introduction)
3. [Purposes](#3-purposes)
4. [Key Features](#4-key-features)
5. [Getting Started](#5-getting-started)
   - 5.1 [Pre-requisites](#51-pre-requisites)
6. [Software Overview](#6-software-overview)
7. [System Requirements](#7-system-requirements)
8. [Important Points](#8-important-points)
9. [Dependencies](#9-dependencies)
   - 9.1 [Run-time Dependency](#91-run-time-dependency)
   - 9.2 [Other Dependency](#92-other-dependency)
10. [How to Setup / Install](#10-how-to-setup--install-python-virtual-environment)
11. [Configuration](#11-configuration)
12. [Maintenance](#12-maintenance)
13. [Monitoring](#13-monitoring)
14. [Disaster Recovery](#14-disaster-recovery)
15. [High Availability](#15-high-availability)
16. [Troubleshooting](#16-troubleshooting)
17. [FAQs](#17-faqs)
18. [Contact Information](#18-contact-information)
19. [References](#19-references)

---

## 1. Author Information
| Author | Created on | Version | Last updated by | Last edited on | Pre Reviewer | L0 Reviewer | L1 Reviewer | L2 Reviewer |
|--------|------------|---------|-----------------|----------------|--------------|-------------|-------------|-------------|
| Hardik Modi | 16-01-2026 | v1.0 | Hardik Modi | 16-01-2026 |  |  |  |  |
---

## 2. Introduction

A Python Virtual Environment is an isolated environment that allows you to install project-specific Python packages and dependencies without affecting the system-wide Python installation.  
The main purpose is to avoid dependency conflicts and keep projects clean, reproducible, and manageable.

---

## 3. Purposes

Python virtual environments are used to solve the following problems:

- Managing different package versions for different projects
- Protecting the system Python from breaking
- Keeping development and production environments consistent
- Simplifying dependency management and deployment

---

## 4. Key Features

- Project-wise isolated Python environment
- Separate package installation per project
- Easy activation and deactivation
- Supports multiple Python versions
- Works with pip, requirements.txt, and dependency tools

---

## 5. Getting Started

### 5.1 Pre-requisites

| Name | Description | Commercial Use | Open Source |
|----|------------|---------------|-------------|
| Python | Python 3.6+ required |  Yes | Yes |
| pip | Python package installer | Yes | Yes |
| venv | Built-in virtual environment module | Yes | Yes |

---

## 6. Software Overview

| Software | Version |
|--------|---------|
| Python | 3.x |
| venv | Built-in |
| virtualenv | Optional |

---

## 7. System Requirements

| Requirement | Minimum Recommendation |
|------------|-----------------------|
| OS | Linux / Windows / macOS |
| RAM | 1 GB |
| Disk Space | 100 MB |
| Python | 3.6 or above |

---

## 8. Important Points

| Point | Description |
|-----|------------|
| Isolation | Each project has its own dependencies |
| Safety | System Python remains untouched |
| Portability | Easy to share via requirements.txt |
| Cleanup | Environment can be deleted anytime |

---

## 9. Dependencies

### 9.1 Run-time Dependency

| Dependency | Version | Description |
|-----------|--------|------------|
| Python | 3.x | Required to run virtual environments |

### 9.2 Other Dependency

| Dependency | Version | Description |
|-----------|--------|------------|
| pip | Latest | Package management |
| setuptools | Latest | Package building |

---

## 10. How to Setup / Install (Python Virtual Environment)

### Step-by-step Installation Instruction

**1. Create virtual environment**
```bash
Sudo apt install python3-venv
python3 -m venv env
```

**2. Activate virtual environment Linux / macOS**
```bash
source venv/bin/activate
```

**3. Activate virtual environment Windows**
****
```bash
venv\Scripts\activate

```
**4. Deactivate virtual environment**
****
```bash
deactivate

```



## 11. Configuration

- The `venv/` directory should not be committed to Git
- Use `requirements.txt` for dependency tracking
- Always activate the environment before running the application

---

## 12. Maintenance

- Regularly update dependencies
- Remove unused packages
- Recreate the environment if dependency conflicts occur

---

## 13. Monitoring

Check installed packages:

    pip list

Freeze dependencies:

    pip freeze > requirements.txt

---

## 14. Disaster Recovery

If the environment gets corrupted, delete the `venv/` directory and recreate it:

    python -m venv venv
    pip install -r requirements.txt

---

## 15. High Availability

Virtual environments support high availability by ensuring:

- Consistent environments across servers
- Same dependency versions in staging and production
- Easy replication in CI/CD pipelines

---

## 16. Troubleshooting

| Issue | Solution |
|------|----------|
| Command not found | Ensure Python is installed |
| Activation failed | Check OS-specific command |
| Package conflict | Recreate virtual environment |

---




## 17. FAQs

**Q1. Why should we use virtual environments?**  
To avoid dependency conflicts and keep projects isolated.

**Q2. Can multiple virtual environments exist?**  
Yes, a separate virtual environment can be created for each project.

**Q3. Is virtual environment mandatory?**  
It is not mandatory but highly recommended for professional Python projects.

**Q4. Can I use virtualenv instead of venv?**  
Yes, virtualenv is an external but more flexible tool.

---


## 18. Contact Information

| Name | Email |
|------|-------|
| Hardik Modi | modihardik19@gmail.com |

---

## 19. References

| Link | Description |
|------|------------|
| https://docs.python.org/3/library/venv.html | Official Python venv documentation |
| https://pip.pypa.io | pip documentation |
| https://virtualenv.pypa.io | virtualenv documentation |
