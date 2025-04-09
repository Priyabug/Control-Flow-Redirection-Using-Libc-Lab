# 🧨 Return-to-libc Attack Lab

> A deep dive into bypassing non-executable stack protections using Return-to-libc attacks.  
> 🔐 Learn how attackers leverage system libraries instead of injecting shellcode.

---

## 📚 Overview

The **Return-to-libc attack** is a powerful exploit technique used when direct shellcode execution is blocked by modern OS protections. Instead of injecting code, attackers redirect execution to existing library functions like `system()` to gain shell access.

---

## 🎯 Objective

Gain hands-on experience with:
- ✅ Buffer overflow vulnerabilities
- ✅ Stack memory layout & calling conventions
- ✅ Return-to-libc exploit construction
- ✅ Linux-based mitigation techniques

---

## 🛠️ Lab Environment

| Tool/Tech           | Version/Info             |
|---------------------|--------------------------|
| OS                  | Ubuntu 20.04 (32-bit preferred) |
| Compiler            | `gcc` with `-fno-stack-protector -z execstack` |
| Debugger            | `gdb` with `peda` plugin |
| Tools               | `readelf`, `objdump`, `python` |

---

## 🧪 Topics Covered

- 💥 Buffer Overflow Vulnerability
- 🧵 Stack Layout & Function Frames
- 🚫 Non-executable Stack Protections
- 🔄 Return-to-libc Technique
- 🧩 Basics of Return-Oriented Programming (ROP)

---

## 📁 Project Structure

```bash
return-to-libc-lab/
├── vulnerable.c        # Program containing buffer overflow
├── Makefile            # Compilation instructions
├── exploit.py          # (Optional) Payload automation script
└── README.md           # Project overview and guide
