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

Offline web shell & backdoor detector for web roots (PHP/ASP/ASPX/JSP/Perl/Python)

---

## ✨ Features

- Offline, strictly read-only scanner for web content roots (PHP / ASP / ASPX / JSP / JSPX / Perl / Python / CGI / .htaccess / web.config) — never executes code
- Known web-shell family signatures: c99, r57, b374k, WSO, China Chopper, weevely, Godzilla, Behinder, AntSword, p0wny, Alfa, IndoXploit, Mini Shell, ASPXSpy, JspSpy ...
- Dangerous sink analysis with user-input taint proximity (eval/assert/system/exec/passthru/shell_exec/popen, preg_replace /e, create_function, call_user_func ...)
- Obfuscation indicators — base64 blobs, gzinflate / str_rot13 / hex / chr() chains, variable functions, string-concatenated function names, char() building
- Static decode layers — safely unwraps base64 / hex / rot13 / gz blobs (pure data, never evaluated) and re-scans the payload for hidden sinks
- Suspicious uploader detection, polyglot images with embedded code, double extensions, handler hijacks
- Shannon entropy + "islands of obfuscation" scoring and recently-modified / anomalous file heuristics
- Per-file malice score (0-100) + A+…F site posture
- MITRE ATT&CK tags (T1505.003, T1027, T1059 ...) and remediation guidance on every finding
- Allowlist of known-good SHA-256 hashes / globs and baseline snapshots with new / modified file diff
- Export TXT / MD / JSON / CSV / SARIF 2.1.0
- Self-test --demo with benign + malicious samples
- Full CLI mode (--path DIR, --fail-on, --json, ...)

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OWebShell
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
