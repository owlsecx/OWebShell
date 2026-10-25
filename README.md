# 🦉 OWebShell

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OWebShell** — Web Shell & Backdoor Detector

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview


OWebShell is an offline web-shell and malicious-code detection tool that scans web directories for backdoors, obfuscated PHP/ASP/JSP payloads and suspicious functions. It applies signature and heuristic analysis, entropy scoring and known-pattern matching to flag likely shells without executing any code. It is intended for authorized incident response and server hardening.

---

## ✨ Features


- Signature and heuristic scanning for PHP/ASP/JSP/Python web shells and backdoors
- Detection of obfuscation (eval/base64/gzinflate chains) and dangerous function calls
- Entropy scoring to surface packed or encoded payloads
- Recursive directory walking with file-type filtering
- Clear risk reporting with per-file findings and structured export
- Offline, non-executing analysis with a --self-test mode

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage


```bash
./OWebShell
./OWebShell --self-test
./OWebShell --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
