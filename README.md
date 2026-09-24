<div align="center">

# Hi, I'm Cristo Fernández Tomé 👋

**Systems & Full-Stack Developer · Rust · C++ · TypeScript · Founder of [SoftDryzz](https://softdryzz.com)**

*From Ring 0 to the browser: I build hypervisors, reverse engineering tooling, security software, CLIs and web platforms.*

[![Website](https://img.shields.io/badge/softdryzz.com-FF5722?style=flat-square&logo=google-chrome&logoColor=white)](https://softdryzz.com)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:contact@softdryzz.com)
[![Available](https://img.shields.io/badge/Available%20for%20projects-00C853?style=flat-square)](#-contact-me)

🌐 *[Leer en Español](README_ES.md)*

</div>

---

## 🚀 About Me

- 🔬 **Low-level first:** Windows kernel drivers, Intel VT-x virtualization and x86-64 internals. I like knowing what the machine is really doing.
- 🕵️ **Reverse engineer:** Static and dynamic analysis of binaries, process memory and network protocols with Ghidra and x64dbg.
- 🔒 **Security builder:** Threat detection, system monitoring, secrets management, licensing and anti-tamper.
- 🦀 **Backend & full-stack:** **Rust**, **C++**, **Java**, **TypeScript** and **Python**, from Tower middleware to React/Svelte frontends and Tauri desktop apps.
- 🤖 **AI & automation:** Local AI agents, LLM integration and workflow automation.

---

## 🧭 What I Work On

| Area | What it covers |
|---|---|
| 🔬 **Systems & Low-Level** | Windows kernel drivers (WDK), Type-1 hypervisors (VMX, EPT, VMCS, VM-exits), x86-64 assembly, Windows internals |
| 🕵️ **Reverse Engineering** | Ghidra, x64dbg, PE triage, unpacking, anti-debug analysis, process memory analysis, network protocol reversing |
| 🔒 **Security Tooling** | Threat detection, system monitoring, secrets management, offline licensing & anti-tamper, Linux server hardening |
| 🦀 **Backend & APIs** | Rust (Axum, Tower, Tokio), Java, Python (FastAPI), PostgreSQL, Redis |
| 🌐 **Frontend & Desktop** | React, Next.js, Svelte, TailwindCSS, Tauri |
| 🎮 **Game Tooling & Modding** | Minecraft server plugins (Paper/Velocity), Meteor Client addons, game memory & protocol analysis |

---

## 📂 Featured Projects

### 🔬 Systems & Reverse Engineering

#### 🌀 Hyperion: Type-1 Hypervisor for Windows

*Intel VT-x hypervisor for Windows x64. Ring 0 kernel driver in C++ plus a Ring 3 loader in Rust, with VM introspection and anti-reversing protection.*

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20ASM-6E4C13?style=flat-square&logo=intel&logoColor=white)
![WDK](https://img.shields.io/badge/WDK-0078D6?style=flat-square&logo=windows&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- ⚙️ **VMX core:** VMCS setup, VM-exit handler, x64 assembly entry stubs and CPUID emulation
- 🧱 **Memory virtualization:** EPT, copy-on-write shadow page tables, MTRR-aware memory typing and deferred INVEPT batching
- 🪝 **EPT hooking & VMI:** Kernel-side VM-exit filtering, execution path tracing and anomaly scoring
- 🔌 **Ring 0 → Ring 3 telemetry:** Async double-buffer pipeline with overflow throttling over an IOCTL gateway, Rust loader
- 📊 **Performance:** Sub-microsecond latency profiling and execution histograms, multi-layer anti-reversing
- 🧪 **Validation:** 5-phase gated deployment with fire-test validation

---

### 🔐 Security & Developer Tools

#### 🔐 [Vaultic v1.4: Secrets Manager](https://github.com/SoftDryzz/vaultic)

*CLI for securely managing secrets and configuration across teams, with Git-based sync. Published on [crates.io](https://crates.io/crates/vaultic).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)

- 🔒 **Strong encryption:** age or GPG with multi-recipient support, no external cloud
- 🌍 **Multi-environment:** dev/staging/prod with smart inheritance, diff and missing-variable detection
- 🚀 **CI/CD ready:** `vaultic ci export` for GitHub/GitLab, `VAULTIC_AGE_KEY`, `--stdout` piping and CI-friendly exit codes
- 📋 **Audit trail:** JSON history of who changed what and when

#### 🛡️ Cerberus v1.0: Security Monitor

*Private security monitor for Windows with real-time threat detection.*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- 🔴 **Process monitor:** Real-time analysis with risk scoring (0-100)
- 🔵 **Executable analyzer:** Hash verification, PE analysis, VirusTotal integration
- 🟢 **Network & system:** Per-process connections, startup items and scheduled tasks
- 🟣 **Alerts & reports:** Native notifications, PDF export, auto-updater, 119 unit tests

#### 🛠️ [ProjectManager v2.0: CLI](https://github.com/SoftDryzz/ProjectManager)

*One command for all your projects. Detects project type and standardizes build/run/test with diagnostics, security and statistics.*

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)

- 🔍 **Auto-detection:** 12+ project types (Gradle, Maven, Node.js, .NET, Python, Rust, Go, Flutter, Docker...)
- 🩺 **Diagnostics & security:** `pm doctor` with A-F scoring, `pm secure` and `pm audit`
- ✅ **800+ tests:** Cross-platform (Windows, Linux, macOS)

---

### 🦀 Rust Crates

#### 🌐 [Tower Rate Tier v0.2](https://github.com/SoftDryzz/tower-rate-tier) · [crates.io](https://crates.io/crates/tower-rate-tier)

*Tier-based rate limiting middleware for Tower. Per-plan limits (free/pro/enterprise), request cost, pluggable storage and standard headers.*

- 📈 **GCRA algorithm** with per-request cost and per-day/custom windows
- 🔌 **Pluggable storage:** In-memory (DashMap) or Redis for multiple servers
- 🎛️ **Customizable:** `on_limited` callback and custom 429 responses, Criterion benchmarks
- 🏗️ **Tower-native:** Axum, Hyper and any Tower service, MSRV 1.75

#### 🧰 [Tower Request Guard v0.1](https://github.com/SoftDryzz/tower-request-guard) · [crates.io](https://crates.io/crates/tower-request-guard)

*Request validation middleware for Tower. Replaces 3-4 separate layers with a single configurable guard.*

- 📏 **Validation:** Max body size, per-route timeouts, Content-Type and required headers
- 💣 **JSON bomb protection:** Max nesting depth validation
- 🧭 **Per-route overrides** plus dry-run `LogAndPass` mode for gradual migration
- 🏗️ **Tower-native:** Axum, Tonic, Hyper or any Tower-based framework

---

## 🛠️ Tech Stack

**Languages**

![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20asm-6E4C13?style=for-the-badge&logo=intel&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Lua](https://img.shields.io/badge/lua-%232C2D72.svg?style=for-the-badge&logo=lua&logoColor=white)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=amazondocumentdb&logoColor=white)

**Systems & Reverse Engineering**

![Windows Driver Kit](https://img.shields.io/badge/WDK-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Intel VT-x](https://img.shields.io/badge/Intel%20VT--x-0071C5?style=for-the-badge&logo=intel&logoColor=white)
![Ghidra](https://img.shields.io/badge/Ghidra-D22128?style=for-the-badge&logoColor=white)
![x64dbg](https://img.shields.io/badge/x64dbg-2B2B2B?style=for-the-badge&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

**Backend & Runtime**

![Tokio](https://img.shields.io/badge/tokio-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/axum-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/tauri-%2324C8DB.svg?style=for-the-badge&logo=tauri&logoColor=%23FFFFFF)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Frontend**

![Svelte](https://img.shields.io/badge/svelte-%23f1413d.svg?style=for-the-badge&logo=svelte&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)

**Data & DevOps**

![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

---

## 💼 What I Can Help With

Available for freelance work and collaborations through [softdryzz.com](https://softdryzz.com):

| Service | Description |
|---|---|
| 🕵️ **Reverse Engineering** | Binary and protocol analysis, software protection review, interoperability research |
| 🔬 **Low-Level Development** | Windows drivers, virtualization, performance-critical Rust/C++ |
| 🔒 **Security Tooling & Hardening** | Monitoring and detection tools, secrets management, server hardening |
| 💻 **Custom Software** | Desktop apps, CLIs, APIs, middleware and integrations |
| 🌐 **Web Development** | Landing pages, web platforms, e-commerce |
| 🧠 **Digital & AI Consulting** | Digitalization plans, AI integration, process automation |

---

## 🎓 Education & Certifications

| Title | Institution |
|---|---|
| **Multi-platform Application Development (DAM)** | Campus Cámara de Comercio de Sevilla |
| **Business Digitalization** | EOI (Escuela de Organización Industrial) |
| **Artificial Intelligence Specialist** | Founderz |

---

## 📈 GitHub Stats

<p align="center">
  <img src="./profile/stats.svg" height="165" alt="GitHub stats" />
  <img src="./profile/top-langs.svg" height="165" alt="Top languages" />
</p>

<p align="center">
  <img src="./profile-3d-contrib/profile-night-rainbow.svg" alt="3D contribution graph" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=SoftDryzz&color=2ea44f&style=flat&label=Profile+Views" alt="Profile views" />
</p>

---

## 📫 Contact Me

[![Website](https://img.shields.io/badge/Website-softdryzz.com-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://softdryzz.com)

| | Email | Purpose |
|---|---|---|
| 📩 | **contact@softdryzz.com** | General inquiries and collaborations |
| 🛡️ | **security@softdryzz.com** | Security vulnerabilities & responsible disclosure |
| ⚖️ | **legal@softdryzz.com** | Commercial licensing |
| 👤 | **cristo@softdryzz.com** | Direct contact |

---

<p align="center">
  <a href="https://github.com/sponsors/SoftDryzz">
    <img src="https://img.shields.io/badge/Sponsor-💗-ea4aaa?style=for-the-badge&logo=github" height="40" alt="GitHub Sponsors">
  </a>
  &nbsp;&nbsp;
  <a href="https://buymeacoffee.com/xtoftomeo" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="40" alt="Buy Me A Coffee">
  </a>
</p>

<p align="center"><i>"Code is like humor. When you have to explain it, it's bad." · Cory House</i></p>

<p align="center"><b>Let's build something awesome together!</b> 🚀</p>
