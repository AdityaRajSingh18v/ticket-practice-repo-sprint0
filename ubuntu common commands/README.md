# 📘 SOP – Common Ubuntu Commands

## 🔹 Document Details

| Author           | Created    | Version | Last updated by  | Last Edited On | Pre Reviewer | L0 Reviewer | L1 Reviewer | L2 Reviewer |
| ---------------- | ---------- | ------- | ---------------- | -------------- | ------------ | ----------- | ----------- | ----------- |
| Aditya Raj Singh | 2026-01-20 | 1.0     | Aditya Raj Singh | 2026-01-20     |              |             |             |             | 

---

## 📑 Table of Contents

1. [Document Details](#-document-details)
2. [Introduction](#1-introduction)
3. [Purpose](#2-purpose)
4. [Scope](#3-scope)
5. [Prerequisites](#4-prerequisites)
6. [File & Content Management Commands](#5-file--content-management-commands)
7. [Directory & Disk Usage](#6-directory--disk-usage)
8. [System Information](#7-system-information)
9. [Process Management](#8-process-management)
10. [Permissions & Ownership](#9-permissions--ownership)
11. [Package Management](#10-package-management)
12. [Service Management](#11-service-management)
13. [Networking (Common Use)](#12-networking-common-use)
14. [User & Session Management](#13-user--session-management)
15. [Utility Commands](#14-utility-commands)
16. [Best Practices](#15-best-practices)
17. [Conclusion](#16-conclusion)
18. [Author](#-author)
19. [Contact Information](#-contact-information)
20. [References](#-references)

---
## 1. Introduction

This document provides a list of **commonly used Ubuntu (Linux) commands** that are frequently used in day-to-day system administration, application support, and DevOps operations.  


---

## 2. Purpose

The purpose of this SOP is to:
- Standardize the usage of common Ubuntu commands
- Help users perform routine operational tasks efficiently
- Serve as a quick reference for system and application support activities

---

## 3. Scope

This SOP applies to:
- Ubuntu-based systems (server and desktop)
- Cloud and on-premise environments
- Support Engineers, System Administrators, and DevOps Engineers

---

## 4. Prerequisites

- Access to an Ubuntu system
- Terminal or SSH access
- User account with appropriate permissions (sudo access where required)

---

## 5. File & Content Management Commands
---
### 🔹cat
#### Description:
Use to Displays the content of a file.

          cat file.txt
### 🔹less
#### Description:
Reads large files page by page.

          less /var/log/syslog
### 🔹head
#### Description:
Displays the first few lines of a file.

          head file.txt
### 🔹tail
#### Description:
Displays the last few lines of a file.
            
          tail file.txt
### 🔹grep
#### Description:
Searches text inside files.

          grep "error" file.txt

---

## 6. Directory & Disk Usage
---
### 🔹du
#### Description:
Shows disk usage of files and directories.

          du -sh /var/log
### 🔹df
#### Description:
Displays filesystem disk usage.

          df -h
---

## 7. System Information
---

### 🔹uptime
#### Description:
Shows how long the system has been running.

          uptime
### 🔹free
#### Description:          
Displays memory and swap usage.

          free -h
---

## 8. Process Management
---

### 🔹ps
#### Description:
Displays running processes.

          ps -ef

### 🔹top
#### Description:
Shows real-time process and resource usage.

          top
### 🔹kill
#### Description:
Terminates a running process using PID.

          kill 1234
          kill -9 1234

---

## 9. Permissions & Ownership
---

### 🔹chmod
#### Description:
Changes file or directory permissions.

          chmod 644 file.txt
          chmod 755 script.sh
### 🔹chown
#### Description:
Changes file ownership.

          sudo chown user:group file.txt

---

## 10. Package Management
---
### 🔹apt update
#### Description:
Updates the package index.

          sudo apt update
### 🔹apt install
#### Description:
Installs packages.

          sudo apt install nginx
### 🔹apt remove
#### Description:
Removes installed packages.

          sudo apt remove nginx
---

## 11. Service Management
---
### 🔹 systemctl status
#### Description:
Checks the status of a service.

          systemctl status nginx

### 🔹 systemctl restart
#### Description:
Restarts a service.

          sudo systemctl restart nginx
---

## 12. Networking (Common Use)
---
### 🔹 ip a
#### Description:
Displays IP address information.

          ip a

### 🔹 ping

#### Description:
Checks network connectivity.

          ping google.com

### 🔹 curl
#### Description:
Tests APIs or fetches URLs.

          curl http://localhost:8080
---

## 13. User & Session Management
---

### 🔹 who
#### Description:
Shows currently logged-in users.

          who

### 🔹 whoami
#### Description:
Displays the current user.

          whoami
---

## 14. Utility Commands
---

### 🔹 history
#### Description:
Shows previously executed commands.

          history

### 🔹 clear
#### Description:
Clears terminal output.

          clear

---         
## 15. Best Practices

- Use `less` instead of `cat` for large files
- Verify process IDs before using `kill -9`
- Regularly monitor disk usage using `df` and `du`
- Use `sudo` only when required

---

## 16. Conclusion

This SOP provides a practical reference for commonly used Ubuntu commands required for daily operational tasks.  
It helps improve efficiency, reduce errors, and maintain standard practices across teams.

## 🔹 Author

| Name             | Role            | Team                 |
| ---------------- | --------------- | -------------------- |
| Aditya Raj Singh | DevOps Trainee | Saarthi |


## 🔹 Contact Information

| Contact Type | Details                                                             |
| ------------ | ------------------------------------------------------------------- |
| Email        | [tadityaraj.singh18@gmail.com](mailto:tadityaraj.singh18@gmail.com) |

---

## 🔹 References

| Links | Descriptions |
|------|-------------|
| https://www.geeksforgeeks.org/linux-unix/25-basic-ubuntu-commands/ | Basic Ubuntu Commands |

