# 📘 SOP – Common Ubuntu Commands

---

## 📌Overview

This document provides a list of **commonly used Ubuntu (Linux) commands** that are frequently used in day-to-day system administration, application support, and DevOps operations.  


---

## 🎯Purpose

The purpose of this SOP is to:
- Standardize the usage of common Ubuntu commands
- Help users perform routine operational tasks efficiently
- Serve as a quick reference for system and application support activities

---

## 📦Scope

This SOP applies to:
- Ubuntu-based systems (server and desktop)
- Cloud and on-premise environments
- Support Engineers, System Administrators, and DevOps Engineers

---

## 🧰Prerequisites

- Access to an Ubuntu system
- Terminal or SSH access
- User account with appropriate permissions (sudo access where required)

---

## 📂File & Content Management Commands
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

## 📂Directory & Disk Usage
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

## 🖥 System Information
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

## ⚙ Process Management
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

## 🔐 Permissions & Ownership
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

## 📦 Package Management
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

## 🔁 Service Management
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

## 🌐 Networking (Common Use)
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

## 🔍 User & Session Management
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

## 🛠 Utility Commands
---

### 🔹 history
#### Description:
Shows previously executed commands.

          history

### 🔹 clear
#### Description:
Clears terminal output.

          clear
