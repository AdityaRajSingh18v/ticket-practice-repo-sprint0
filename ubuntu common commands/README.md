#  SOP – Common Ubuntu Commands

##  Document Details

| Author           | Created    | Version | Last updated by  | Last Edited On |L0 Reviewer | L1 Reviewer | L2 Reviewer |
| ---------------- | ---------- | ------- | ---------------- | -------------- | ----------- | ----------- | ----------- |
| Aditya Raj Singh | 2026-01-20 | 1.0     | Aditya Raj Singh | 2026-01-20     | Mohit kumar  | Pritam      |  Abhishek Dubey / Ravindra Kumar    | 

---

##  Table of Contents


1. [Introduction](#1-introduction)
2. [Purpose](#2-purpose)
3. [Scope](#3-scope)
4. [Pre-requisites](#4-pre-requisites)
5. [Environment Verification](#5-environment-verification)
6. [Command Reference](#6-command-reference)
   - [File Operations](#61-file-operations)
   - [User & Permission Commands](#62-user--permission-commands)
   - [System Monitoring](#63-system-monitoring)
   - [Process & Service Commands](#64-process--service-commands)
   - [Network Commands](#65-network-commands)
   - [Search & Text Processing](#66-search--text-processing)
   - [Package Management (Linux Admin Work)](#67-package-management-linux-admin-work)
   - [Compression & Archives](#68-compression--archives)
7. [Conclusion](#7-conclusion)
8. [References](#8-references)
9. [Contact Information](#9-contact-information)


---

## 1. Introduction

This document provides a Standard Operating Procedure (SOP) for frequently used Linux commands. It helps users perform basic system tasks such as monitoring system health, managing files, validating network connectivity, and controlling running processes.

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

## 4. Pre-requisites

| Requirement | Description |
|-------------|-------------|
| Operating System | Linux-based system |
| User Access | Valid login credentials |
| Privileges | Sudo access when required |
| Terminal | Command-line interface |
| Basic Knowledge | Familiarity with Linux shell |

---

## 5. Environment Verification

| Command | Description | Example |
|--------|-------------|---------|
| `whoami` | Displays current user | `whoami` |
| `echo $SHELL` | Shows active shell | `/bin/bash` |
| `ls --version` | Verifies command availability | `ls (GNU coreutils) 9.1` |

---

## 6. Command Reference


### 6.1 File Operations

| Command | Description | Example |
|--------|-------------|---------|
| `pwd` | Displays current directory | `/home/ubuntu/projects` |
| `ls -lh` | Lists files in detail | `config.yml 2K README.md 5K` |
| `mkdir <dir>` | Creates directory | `mkdir logs` |
| `touch <file>` | Creates empty file | `touch notes.txt` |
| `cp <src> <dest>` | Copies file | `cp report.txt backup.txt` |
| `mv <src> <dest>` | Renames/moves file | `mv old.log new.log` |
| `rm <file>` | Deletes file | `rm temp.txt` |
| `cat <file>` | Displays file content | `cat notes.txt → Hello World` |
| `nano file` | Opens a file in the Nano editor for simple command-line editing. | `nano nginx.conf` |
| `vi file` | Opens a file in the Vim editor for advanced editing. | `vi docker-compose.yml` |



### 6.2 User & Permission Commands

| Command | Description | Example |
|--------|-------------|---------|
| `whoami` | Shows logged-in user | `ubuntu` |
| `id <user>` | Displays user identity | `id ubuntu → uid=1000` |
| `groups` | Shows user groups | `groups → sudo docker` |
| `chmod <mode> <file>` | Changes permissions | `chmod 755 app.sh` |
| `chown <user>:<grp> <file>` | Changes ownership | `chown root:root config.conf` |
| `passwd <user>` | Changes password | `passwd devuser` |



### 6.3 System Monitoring

| Command | Description | Example |
|--------|-------------|---------|
| `uptime` | Shows system running time | `uptime → 2:10 up 3 days, load average: 0.05` |
| `free -h` | Displays memory usage | `free -h → Mem: 7.7Gi used` |
| `df -h` | Shows disk utilization | `df -h → /dev/sda1 40% used` |
| `top` | Displays live processes | `top → PID 1203 nginx using CPU` |
| `hostname` | Shows system name | `hostname → web-server-01` |



### 6.4 Process & Service Commands

| Command | Description | Example |
|--------|-------------|---------|
| `ps aux` | Lists running processes | `nginx PID 1234 running` |
| `kill <pid>` | Terminates process | `kill 1234` |
| `systemctl status <svc>` | Shows service status | `systemctl status nginx → active` |
| `systemctl restart <svc>` | Restarts service | `systemctl restart nginx` |



### 6.5 Network Commands

| Command | Description | Example |
|--------|-------------|---------|
| `ip a` | Displays IP addresses | `eth0 → 192.168.1.10` |
| `ping <host>` | Tests connectivity | `ping google.com → time=20ms` |
| `curl <url>` | Tests HTTP endpoint | `curl http://localhost:8080/health` |
| `ss -tunlp` | Shows listening ports | `LISTEN 0.0.0.0:22` |
| `hostname -I` | Shows system IP | `192.168.1.10` |



## 6.6 Search & Text Processing

| Command | Description | Example |
|--------|-------------|---------|
| `grep "text" file` | Searches for a specific text pattern inside a file. Commonly used in log analysis. | `grep "ERROR" app.log` |
| `grep -R "text" /path` | Recursively searches for text in all files under a directory. | `grep -R "db_host" /etc` |
| `awk '{print $1}' file` | Extracts and prints a specific column from a file (column-based processing). | `awk '{print $1}' users.txt` |
| `sed 's/old/new/g' file` | Replaces all occurrences of a text pattern in a file. | `sed 's/http/https/g' config.txt` |
| `wc -l file` | Counts the number of lines in a file. | `wc -l access.log` |
| `sort file` | Sorts the contents of a file in alphabetical order. | `sort names.txt` |
| `uniq` | Removes duplicate consecutive lines (usually used with sort). | `sort names.txt | uniq` |



## 6.7 Package Management (Linux Admin Work)

### Ubuntu / Debian

| Command | Description | Example |
|--------|-------------|---------|
| `apt update` | Updates the local package index with the latest available packages. | `sudo apt update` |
| `apt install nginx` | Installs the specified package on the system. | `sudo apt install nginx` |
| `apt remove nginx` | Removes the installed package but keeps configuration files. | `sudo apt remove nginx` |

### RHEL / CentOS

| Command | Description | Example |
|--------|-------------|---------|
| `yum install nginx` | Installs a package on RHEL/CentOS 7 and 8 systems using YUM. | `sudo yum install nginx` |
| `dnf install nginx` | Installs a package on RHEL/CentOS 9 systems using DNF. | `sudo dnf install nginx` |



## 6.8 Compression & Archives

| Command | Description | Example |
|--------|-------------|---------|
| `tar -cvf file.tar dir` | Creates a TAR archive from a directory or files. | `tar -cvf backup.tar logs/` |
| `tar -xvf file.tar` | Extracts files from a TAR archive. | `tar -xvf backup.tar` |
| `tar -czvf file.tar.gz dir` | Creates a compressed TAR.GZ archive. | `tar -czvf app.tar.gz app/` |
| `unzip file.zip` | Extracts contents of a ZIP archive. | `unzip release.zip` |
| `zip -r file.zip dir` | Creates a ZIP archive recursively from a directory. | `zip -r project.zip project/` |

---

## 7. Conclusion

This SOP provides a structured and practical reference for commonly used Ubuntu/Linux commands required for daily operational, administrative, and troubleshooting tasks. By following standardized command usage, users can work more efficiently, reduce errors, and maintain consistency across environments. This document serves as a quick guide for support engineers, system administrators, and DevOps professionals in real-world scenarios.

---

## 8. References

| Description | Link |
|------------|------|
| Linux manual pages (official) | [https://man7.org/linux/man-pages/](https://man7.org/linux/man-pages/) |
| Ubuntu official documentation | [https://help.ubuntu.com/](https://help.ubuntu.com/) |
| Linux basic commands reference | [https://www.geeksforgeeks.org/linux-unix/](https://www.geeksforgeeks.org/linux-unix/) |
| Linux command line fundamentals | [https://linuxcommand.org/](https://linuxcommand.org/) |

---

## 9. Contact Information

| Name             | Team                 | Contact Type | Details                                                                               |
| ---------------- | -------------------- | ------------ | ------------------------------------------------------------------------------------ |
| Aditya Raj Singh | Saarthi              |Email        | [aditya.singh.snaatak@mygurukulam.co](mailto:aditya.singh.snaatak@mygurukulam.co) |

---

