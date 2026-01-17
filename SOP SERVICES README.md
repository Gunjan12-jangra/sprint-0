# Standard Operating Procedure (SOP's) for systemctl
## Step by step guide to start, stop, enable, disable, and check status of services using systemctl on Ubuntu

---

## Table of Contents

1. Introduction
2. Features
3. Purpose
4. Pre-requisites
5. How to Run systemctl Commands
6. Service Management using systemctl (with Examples)
7. Start Service
8. Stop Service
9. Restart Service
10. Enable Service
11. Disable Service
12. Check Service Status
13. Troubleshooting
14. Summary

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

## Types of Services (Internal vs External)
### 1. Internal Service (System/Internal Service)

Internal services are core system services required for the operating system to function properly. These services usually start automatically at boot time and are managed by the OS.

Example: ssh

#### Use case:

- Remote server access
- System administration

### 2. External Service (User-installed / Application Service)

External services are installed by users or administrators to provide additional functionality such as web servers, databases, or container runtimes.

Example: nginx

#### Use case:

- Web hosting
- Reverse proxy
- Load balancing
  
---

## Service Management using systemctl

### 1. External Service Example: nginx

#### 1. Start a Service

Used to start a service immediately.

```bash
sudo systemctl start nginx
```

#### 2. Stop a Service

Used to stop a running service.

```bash
sudo systemctl stop nginx
```

<img width="1847" height="494" alt="image" src="https://github.com/user-attachments/assets/337575de-48d6-4273-a48d-d762da9c6678" />

---

#### 3. Restart a Service

Used to stop and start the service again.

```bash
sudo systemctl restart nginx
```

<img width="1759" height="706" alt="image" src="https://github.com/user-attachments/assets/ed893c5f-d1d5-4ab9-b793-5aa3a462b3a2" />

---
#### 6. Enable a Service (Start on Boot)

Used to start the service automatically when the system boots.

```bash
sudo systemctl enable nginx
```

#### 5. Disable a Service (Do Not Start on Boot)

Used to prevent the service from starting at boot.

```bash
sudo systemctl disable nginx
```

<img width="1568" height="319" alt="image" src="https://github.com/user-attachments/assets/7abe3bd5-fb14-4a79-aecb-d2082c788a58" />

---

#### 6. Check Service Status

Used to check whether the service is running or stopped.

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

## Author

| Name             | Role            | Team                 |
| ---------------- | --------------- | -------------------- |
| Gunjan Jangra | DevOps Trainee | Saarthi |










    
