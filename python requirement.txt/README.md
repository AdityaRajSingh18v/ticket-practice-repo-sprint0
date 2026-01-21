#  📑Python `requirements.txt` Documentation

##  Table of Contents
1. [Introduction](#introduction)
2. [Why `requirements.txt` is Required](#why-requirementstxt-is-required)
3. [Use Cases of `requirements.txt`](#use-cases-of-requirementstxt)
4. [Structure of `requirements.txt`](#structure-of-requirementstxt)
5. [Dependency Versioning](#dependency-versioning)
6. [Best Practices for Dependency Versioning](#best-practices-for-dependency-versioning)
7. [Installing Dependencies](#installing-dependencies)
8. [Security Considerations](#security-considerations)
9. [Summary](#summary)

---

## 📌 Introduction

In any Python-based application, managing external libraries and packages is a critical part of development and deployment.  
The `requirements.txt` file is used to **define, manage, and install all Python dependencies** required for an application to run consistently across different environments such as **development, testing, staging, and production**.

This file ensures that every developer, CI/CD pipeline, and server uses the **same dependency versions**, avoiding unexpected issues caused by mismatched libraries.

---

##  Why `requirements.txt` is Required

Python applications rarely work in isolation. They rely on multiple third-party libraries such as web frameworks, database drivers, authentication libraries, and utility packages.

`requirements.txt` is required because:

- It provides a **single source of truth** for all Python dependencies  
- It ensures **environment consistency** across local machines and servers  
- It simplifies **application setup and onboarding**  
- It enables **automated dependency installation** in CI/CD pipelines  
- It helps avoid **“works on my machine”** problems  

Without a proper `requirements.txt`, applications become difficult to reproduce and maintain.

---

##  Use Cases of `requirements.txt`

### 1️⃣ Local Development
Developers can quickly set up the project by installing all dependencies using a single command:

```bash
pip install -r requirements.txt

