# Log Rotation Management using Logrotate (Ubuntu)

🔹 Document Details

| Author            | Created    | Version | Last updated by  | Last Edited On | Pre Reviewer | L0 Reviewer | L1 Reviewer | L2 Reviewer |
| ----------------- | -------------- | ------- | ---------------- | -------------- | ------------ | ----------- | ----------- | ----------- |
| Aditya Raj Singh  | 2026-01-20 | 1.0     | Aditya Raj Singh | 2026-01-20     |              |             |             |            

---
# SOP – Log Rotation Management using Logrotate (Ubuntu)

## 1. Introduction

The purpose of this SOP is to define the standard procedure for configuring and managing log rotation on Ubuntu servers using the **logrotate** utility.

**Logrotate** helps control log file growth, ensures efficient disk space utilization, and maintains system stability by automatically rotating, retaining, compressing, and removing log files.

## 2. Purpose

The objectives of this SOP are to:

- Configure automated log rotation for system and application logs
- Define log rotation frequency (daily, weekly, size-based, etc.)
- Implement retention policies to control log history
- Prevent disk space exhaustion and service failures
- Follow logging best practices for production environments

## 3. Scope

This SOP applies to:

- Ubuntu-based servers (Development, QA, UAT, Production)
- System logs (syslog, auth.log, etc.)
- Application and service logs
- On-premise and cloud-hosted Ubuntu instances


## 5. Prerequisites

- Ubuntu operating system installed
- Root or sudo access
- Logrotate package installed (default on Ubuntu)
- Identified log file paths

**Verify installation:**

          logrotate --version

## 6. Logrotate Configuration Overview

Logrotate configuration on Ubuntu is managed at **two levels**:

- **Global configuration:** `/etc/logrotate.conf`
- **Service/Application-specific configuration:** `/etc/logrotate.d/`

**Best practice:** Create a separate configuration file for each application.


## 7. Procedure

### 7.1 Global Configuration Verification

**Global configuration file:** `/etc/logrotate.conf`

This file defines default behavior such as:
- Rotation frequency
- Retention count
- Compression settings

### 7.2 Application Logrotate Configuration

**Step 1: Identify the Log File**

          Example: /var/log/myapp/app.log

Step 2: Create Logrotate Configuration File


          sudo nano /etc/logrotate.d/myapp
