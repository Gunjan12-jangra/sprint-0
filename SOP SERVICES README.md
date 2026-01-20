# Standard Operating Procedure (SOP's) for systemctl
## Managing Services Using systemctl on Ubuntu 

---

## Authors

| Author           | Created    | Version | Last updated by  | Last Edited On | Pre Reviewer | L0 Reviewer | L1 Reviewer | L2 Reviewer |
| ---------------- |---------------- | ------- | ---------------- | -------------- | ------------ | ----------- | ----------- | ----------- |
| Gunjan Jangra  |  18-01-2026    |  1.0     | Gunjan Jangra |  18-01-2026     |              |             |             |             |

---

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Purpose](#purpose)
4. [Pre-requisites](#pre-requisites)
5. [Software Overview](#software-overview)
6. [System Requirement](#system-requirement)
7. [Dependencies](#dependencies)
8. [Service Management using systemctl (with Example)](#service-management-using-systemctl-with-example)
9. [Troubleshooting](#troubleshooting)
10. [Summary](#summary)
11. [Contact Information](#contact-information)
12. [References](#references)

---

## Introduction

Systemctl is a command-line tool used to manage services on Linux systems that use systemd.
Using systemctl, we can start, stop, restart, enable, disable, and check the status of services).
With systemctl, services can be controlled temporarily (runtime) or permanently (persist across system reboots).

---

## Features

Systemctl provides the following features:

- Start and stop services easily

- Restart services without rebooting the system

- Enable services to start automatically at boot

- Disable services from starting at boot

- Check service status and health

- Manage system and application services

---

## Purpose

Systemctl is used to:

- Manage Linux services efficiently

- Control service startup and shutdown

- Monitor service status for troubleshooting

- Maintain stable server operations

- Simplify service management for beginners

---

## Pre-requisites

| Requirement | Description                                          |
| ------------ | ---------------------------------------------------- | 
| OS Access  | User must have access to Linux system | 
| Privileges  | sudo or root access required | 

---

## Software Overview

| Software | Description                                          |
| ------------ | ---------------------------------------------------- | 
| systemctl	| Command-line utility to control systemd services | 

---

## System Requirement

| Requirement |	Minimum Recommendation |
| ------------ | ---------------------------------------------------- | 
| OS	| Linux with systemd (Ubuntu 18.04+) |
| RAM |	1 GB or higher |
| Disk |	5 GB or higher |

---

## Dependencies
| Dependency | Description	 |
| ------------ | ---------------------------------------------------- | 
| systemd |	Init system and service manager |


➡️ Note: Most modern Linux distributions come with systemd installed by default.

---

## Service Management using systemctl

### 1. Start a Service

Used to start a service immediately.

#### Syntax: 

```bash
systemctl start <service-name>
```
#### Example

```bash
sudo systemctl start nginx
```

---

### 2. Stop a Service

Used to stop a running service.

#### Syntax: 

```bash
systemctl stop <service-name>
```
#### Example

```bash
sudo systemctl stop nginx
```

<img width="1847" height="494" alt="image" src="https://github.com/user-attachments/assets/337575de-48d6-4273-a48d-d762da9c6678" />

---

### 3. Restart a Service

Used to stop and start the service again.

#### Syntax: 

```bash
systemctl restart <service-name>
```

#### Example

```bash
sudo systemctl restart nginx
```

<img width="1759" height="706" alt="image" src="https://github.com/user-attachments/assets/ed893c5f-d1d5-4ab9-b793-5aa3a462b3a2" />

---
### 6. Enable a Service (Start on Boot)

Used to start the service automatically when the system boots.

#### Syntax: 

```bash
systemctl enable <service-name>
```
#### Example

```bash
sudo systemctl enable nginx
```

---

### 5. Disable a Service (Do Not Start on Boot)

Used to prevent the service from starting at boot.

#### Syntax: 

```bash
systemctl disable <service-name>
```

#### Example

```bash
sudo systemctl disable nginx
```

<img width="1568" height="319" alt="image" src="https://github.com/user-attachments/assets/7abe3bd5-fb14-4a79-aecb-d2082c788a58" />

---

### 6. Check Service Status

Used to check whether the service is running or stopped.

#### Syntax: 

```bash
systemctl status <service-name>
```

#### Example

```bash
sudo systemctl status nginx
```

<img width="1782" height="759" alt="image" src="https://github.com/user-attachments/assets/ef25f73c-9b51-4f84-8d0c-cb4f9d8f6176" />

---

## Troubleshooting

| Issue | Solution	 |
| ------------ | ---------------------------------------------------- | 
| Service not starting | Check systemctl status nginx	 |
| Permission denied | Use sudo |
| Service not found | Verify service name |

---

## Summary

Systemctl is a powerful and essential Linux utility used to manage system services efficiently. 
It provides administrators with full control over both internal and external services, ensuring reliable system operations and service availability.

---

## Contact Information

| Contact Type | Details                                                             |
| ------------ | ------------------------------------------------------------------- |
| Email        | [jangragunjan39@gmail.com](mailto:jangragunjan39@gmail.com) |

---

## References

| Reference                 | Link                                                             |
| ------------------------- | ---------------------------------------------------------------- |
| Linux Man Pages – systemctl   |      https://man7.org/linux/man-pages/man1/systemctl.1.html |
| DigitalOcean Community Tutorial     | https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units  |

---










    
