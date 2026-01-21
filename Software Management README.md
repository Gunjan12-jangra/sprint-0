# Standard Operating Procedure (SOP's) for APT
## Managing Software Packages Using APT on Ubuntu

---

## Authors

| Author           | Created    | Version | Last updated by  | Last Edited On | Pre Reviewer | L0 Reviewer | L1 Reviewer | L2 Reviewer |
| ---------------- |---------------- | ------- | ---------------- | -------------- | ------------ | ----------- | ----------- | ----------- |
| Gunjan Jangra  |  19-01-2026    |  1.0     | Gunjan Jangra |  19-01-2026     |              |             |             |             |

---

## Table of Contents

## Index

## Index

1. [Introduction](#introduction)  
2. [Features](#features)  
3. [Purpose](#purpose)  
4. [Pre-requisites](#pre-requisites)  
5. [Software Overview](#software-overview)  
6. [System Requirement](#system-requirement)  
7. [Dependencies](#dependencies)  
8. [Package Management using APT](#package-management-using-apt)  
9. [Troubleshooting](#troubleshooting)  
10. [Summary](#summary)  
11. [Contact Information](#contact-information)  
12. [References](#references)  

---

## Introduction

APT (Advanced Package Tool) is a command-line package management system used in Ubuntu.
Using APT, users can install, update, upgrade, and remove software packages efficiently with commonly used flags to automate tasks.

---

## Features

APT provides the following features:

- Install software packages easily

- Update package index from repositories

- Remove software packages with or without configuration files

- Support flags for automation and quiet operation

---

## Purpose

APT is used to:

- Install required software on Ubuntu systems

- Keep system packages updated

- Remove unwanted or unnecessary software

- Automate package management tasks using flags

---

## Pre-requisites

|  Requirement     | Description   |
|-----------------|--------------|
| OS Access  | User must have access to Ubuntu system   | 
| Privileges | sudo or root access required |
| Internet | Required for downloading packages from repositories |

---

## Software Overview

|  Software	    | Description   |
|-----------------|--------------|
| apt |	Command-line package manager for Ubuntu system |

---

## System Requirement

| Requirement	 | Minimum Recommendation |
|-----------------|--------------|
| OS	 | Ubuntu 18.04 or higher |
| RAM |	1 GB or higher |
| Disk |	5 GB or higher |

---

## Dependencies

| Dependency |	Description |
|-----------------|--------------|
| dpkg |	Low-level package management system |

---

## Package Management using APT

### 1. Update Package List

Used to update the local package index from repositories.

➡️ Note: APT internally uses dpkg for installing, removing, and managing packages.

#### Syntax:

```bash
apt update [options]
```

#### Common Flags:

- -y : Automatically answer yes to prompts

- -q : Quiet mode (minimal output)

- --assume-yes : Automatically assume “yes” for all prompts

#### Example:

```bash
sudo apt update -y -q
```

<img width="1472" height="558" alt="image" src="https://github.com/user-attachments/assets/1e9c73b8-1738-4039-86c7-bac5ad835326" />

 ---

 ### 2. Install a Package

Used to install a software package.

#### Syntax:

```bash
apt install <package-name> [options]
```

#### Common Flags:

- -y : Automatically confirm installation
  
- --no-install-recommends : Skip recommended packages
  
- -q : Minimal output

- --reinstall : Reinstall package if already installed

- -f / --fix-broken : Fix broken dependencies


#### Example:

```bash
sudo apt install nginx -y --no-install-recommends
```

<img width="1578" height="581" alt="image" src="https://github.com/user-attachments/assets/d9785309-1fac-4043-b505-c912661b84e5" />

---

### 3. Remove a Package

Used to remove an installed software package while keeping configuration files.

#### Syntax:

```bash
apt remove <package-name> [options]
```

#### Common Flags:

- -y : Automatically confirm removal

- -q : Quiet mode

#### Example:

```bash
sudo apt remove nginx -y -q
```

<img width="1406" height="495" alt="image" src="https://github.com/user-attachments/assets/f538b5c2-2c43-4800-a9b9-ff40e80a59b5" />

---


### 4. Remove Package with Configuration Files

Used to completely remove a package along with its configuration files.

#### Syntax:

```bash
apt purge <package-name> [options]
```

#### Common Flags :
- -y : Automatically confirm purge

- -q : Quiet mode

#### Example:

```bash
sudo apt purge nginx -y -q
```

<img width="1561" height="550" alt="image" src="https://github.com/user-attachments/assets/f82ff832-4db1-4ab8-bc97-acf73183bb61" />

---

## Troubleshooting
| Issue |	Solution |
|------ | ----- |
| Package not found |	Verify package name spelling |
| Permission denied |	Use sudo for elevated privileges |
| Update fails |	Run sudo apt update again or check internet connectivity |

---

## Summary

APT is an essential and powerful package management tool in Ubuntu systems.
It allows users to install, update, upgrade, remove, and clean packages efficiently using common flags for automation and quiet execution.

---

## Contact Information

| Contact Type | Details                                                             |
| ------------ | ------------------------------------------------------------------- |
| Email        | [jangragunjan39@gmail.com](mailto:jangragunjan39@gmail.com) |

---

## References

| Reference | Link |
| ----- | ----- |
| Linux Man Pages-apt |https://manpages.ubuntu.com/manpages/resolute/en/man8/apt.8.html?utm_source |
| Ubuntu Documentation |	https://help.ubuntu.com/community/Apt |

---
