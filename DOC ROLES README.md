# Ansible Role | Directory Structure

## Document Details
---

| Author | Created on | Last updated by |	Last edited on |
|-------- | ---------| -------- | -------- |
| Gunjan |	19-01-2026 |	Gunjan |	19-01-2026 |

---

## Index

1. [Introduction](#introduction)
2. [Role Directory Structure](#role-directory-structure)
3. [Purpose of Each Directory](#purpose-of-each-directory)
4. [Usage Example](#usage-example)
5. [Troubleshooting](#troubleshooting)
6. [References](#references)
7. [End Note](#end-note)

---

## Introduction

Ansible Roles help us organize and structure our automation work in a clean, reusable, and scalable way.
They provide a well-defined directory structure to group tasks, variables, templates, and files, making playbooks easier to read, maintain, and reuse across multiple projects or servers. 
Roles are widely used in DevOps environments for efficient configuration management and application deployment.

---

## Role Directory Structure

```
roles/
└── my_role/
    ├── defaults/
    │   └── main.yml
    ├── vars/
    │   └── main.yml
    ├── tasks/
    │   └── main.yml
    ├── handlers/
    │   └── main.yml
    ├── files/
    ├── templates/
    ├── meta/
    │   └── main.yml
    ├── tests/
    │   ├── inventory
    │   └── test.yml
    └── README.md
```

---

## Purpose of Each Directory

### defaults/

- Contains default variable values for the role.
- Variables here have the lowest priority in Ansible variable precedence.
- Values can be overridden via inventory, playbooks, or extra variables.
- Recommended place for all configurable options.

**Example use case:** Default ports, package versions, feature flags.

---

### vars/

- Stores role-specific variables with higher priority than defaults.
- Not intended to be overridden frequently.
- Used when values must remain constant.

**Example use case:** Internal paths, OS-specific constants.

---

### tasks/

- Contains the logic of the role.
- `main.yml` is the entry point and may include other task files.
- Tasks execute sequentially.

**Example use case:** Installing packages, configuring services, deploying applications.

---

### handlers/

- Special tasks executed only when notified.
- Prevent unnecessary repeated operations.

**Example use case:** Restarting or reloading a service after config change.

---

### files/

- This folder holds static files that are copied directly to the target servers.
- These files are usually used with the copy module in tasks.

 **Example use case:** Scripts, binaries, or configuration files that don’t need any changes.

---

### templates/

* Contains Jinja2 template files (`.j2`).
* Supports variables, conditionals, and loops.

**Example use case:** Dynamic configuration files.

---

### meta/

* Holds role metadata.
* Defines dependencies, supported platforms, and Ansible version.

**Example use case:** Declaring dependent roles for automatic installation.

---

### tests/

- Used for testing and validation of the role.
- Helpful for CI/CD pipelines.

**Example use case:** Verifying role behavior before production use.

---

### README.md

- Official documentation for the role.
- Describes variables, usage, and examples.

---

## Usage Example

```yaml
- hosts: webservers
  roles:
    - my_role
```

---

## Troubleshooting

| Issue                 | Solution                            |
| --------------------- | ----------------------------------- |
| Role not found        | Verify roles_path or directory name |
| Variables not applied | Check variable precedence           |
| Handler not executed  | Ensure `notify` is defined in tasks |

---

## References

| Link                                                                                                                                                           | Description                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------ |
| [https://docs.ansible.com/](https://docs.ansible.com/)                                                                                                         | Official Ansible Documentation |
| [https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html) | Ansible Roles Guide            |

---

## End Note

This document provides a clear explanation of the Ansible Role directory structure and the purpose of each directory. 

