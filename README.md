# 🧠 Linux Privilege Escalation Lab


---

## 🧩 Overview

This project documents a deep-dive into **Linux Privilege Escalation techniques** — from enumeration to kernel exploits, SetUID abuse, and shared library manipulation — culminating in a hands-on **Lab Skills Test** with Docker containers.

Each step includes clear demonstrations, reasoning, and screenshots that validate real exploit execution on the **UWECyber VM**.

---

## ⚙️ Table of Contents

1. [Enumeration](#-enumeration)
2. [Kernel Exploits](#-kernel-exploits)
3. [Vulnerable Packages](#-vulnerable-packages)
4. [Cron Abuse](#-cron-abuse)
5. [SetUID Exploitation](#-setuid-exploitation)
6. [GTFOBins](#-gtfobins)
7. [Sudo Abuse](#-sudo-abuse)
8. [PATH Variable Abuse](#-path-variable-abuse)
9. [Shared Libraries & LD_PRELOAD](#-shared-libraries--ld_preload)
10. [Shared Library Privilege Escalation](#-shared-library-privilege-escalation)
11. [Lab Skills Test](#-lab-skills-test)
   - Flag 1–5 walkthroughs

---

## 🔍 Enumeration

Command used:

```bash
find / -readable -user uwe 2>/dev/null | head -n 10

