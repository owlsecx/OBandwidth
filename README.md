# 🦉 OBandwidth

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OBandwidth** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OBandwidth measures network throughput on Linux. It samples per-interface traffic from /proc/net/dev, keeps a history with live sparkline graphs, and grades link health based on saturation, errors and drops. It can also diff offline /proc/net/dev snapshots, run a loopback TCP throughput test and rank top talkers from ss or netstat output.

---

## ✨ Features

- Per-interface RX/TX rates from /proc/net/dev with configurable interval and sample count
- Live sparkline graphs and throughput history
- Link-health grading for saturation, errors and drops
- Offline mode: diff two /proc/net/dev snapshots to calculate rates
- Loopback TCP throughput test with configurable size and chunk
- Top-talker ranking from ss/netstat output; reports in TXT / Markdown / JSON / CSV / SARIF

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OBandwidth                                 # interactive menu
./OBandwidth --count 5 --interval 2 --format md
./OBandwidth --proc a.txt --proc2 b.txt --format json
./OBandwidth --test --size 512 --chunk 128
./OBandwidth --talkers ss.txt
```

Run `./OBandwidth --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
