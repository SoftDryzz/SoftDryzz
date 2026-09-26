<div align="center">


**Systems & Full-Stack Developer · C++ · Rust · TypeScript · Founder of [SoftDryzz](https://softdryzz.com)**

*From Ring 0 to the browser: I build hypervisors, reverse engineering tooling, security software, CLIs and web platforms.*

[![Website](https://img.shields.io/badge/softdryzz.com-FF5722?style=flat-square&logo=google-chrome&logoColor=white)](https://softdryzz.com)
[![Blog](https://img.shields.io/badge/Blog-111111?style=flat-square&logo=rss&logoColor=white)](https://softdryzz.com/blog/)
[![crates.io](https://img.shields.io/badge/crates.io-3%20crates-E6B14C?style=flat-square&logo=rust&logoColor=white)](https://crates.io/crates/vaultic)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:contact@softdryzz.com)
[![Available](https://img.shields.io/badge/Available%20for%20projects-00C853?style=flat-square)](#-contact-me)

🌐 *[Leer en Español](README_ES.md)*

</div>

---

## ⚡ At a Glance

| | |
|---|---|
| 🔬 **Low-level** | Windows kernel drivers (WDK) · Type-1 hypervisor on Intel VT-x/EPT · x86-64 assembly |
| 🕵️ **Reverse engineering** | Ghidra · x64dbg · WinDbg · PE triage · isolated analysis lab |
| 🦀 **Open source** | 3 crates on crates.io · 40 public releases · 800+ tests in ProjectManager |
| 🧾 **Business software** | VeriFactu e-invoicing and a FIFO/IRPF capital-gains engine for the Spanish market |
| 📦 **Portfolio** | 50+ repositories · top languages by volume: C++, Java, Rust, TypeScript |

## 🔭 Right Now

- 🧾 Building a **VeriFactu-compliant e-invoicing application** (Rust · Axum · Tauri · SvelteKit)
- 📈 Building a **capital-gains tax engine** (FIFO / Spanish IRPF) for tax advisors
- ✍️ Writing a blog series on x86 privilege rings: [Ring 0](https://softdryzz.com/blog/posts/de-ring-3-a-ring-0) → [Ring -1](https://softdryzz.com/blog/posts/ring-menos-1-hipervisor) → Ring -2 (SMM) next
- 🛠️ Shipped [ProjectManager v2.1](https://github.com/SoftDryzz/ProjectManager/releases) (September 2026)

---

## 🧭 What I Work On

| Area | What it covers |
|---|---|
| 🔬 **Systems & Low-Level** | Windows kernel drivers (WDK), Type-1 hypervisors (VMX, EPT, VMCS, VM-exits), x86-64 assembly, Windows internals |
| 🕵️ **Reverse Engineering** | Ghidra, x64dbg, WinDbg, PE triage, unpacking, anti-debug analysis, process memory analysis, network protocol reversing |
| 🔒 **Security Tooling** | Threat detection, system monitoring, secrets management, offline licensing & anti-tamper, Linux server hardening |
| 🧾 **Regulated Business Software** | Spanish e-invoicing (VeriFactu / AEAT), tax calculation engines, audit trails |
| 🦀 **Backend & APIs** | Rust (Axum, Tower, Tokio), Java, Python (FastAPI), PostgreSQL, Redis |
| 🌐 **Frontend, Desktop & Mobile** | React, Next.js, Svelte/SvelteKit, TailwindCSS, Tauri, Flutter |
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
- 🧱 **Memory virtualization:** EPT with MTRR-aware memory typing and deferred INVEPT batching
- 🔌 **Ring 0 → Ring 3 telemetry:** async double-buffer pipeline over an IOCTL gateway, Rust loader

<details>
<summary><b>More internals</b></summary>

- 🧱 Copy-on-write shadow page tables and 4 KB split paging
- 🪝 **EPT hooking & VMI:** kernel-side VM-exit filtering, execution path tracing and anomaly scoring
- 📊 **Performance:** sub-microsecond latency profiling and execution histograms, multi-layer anti-reversing
- 🧪 **Validation:** 5-phase gated deployment with fire-test validation, tested under nested virtualization

</details>

### 🔐 Security & Developer Tools

#### 🔐 [Vaultic v1.4: Secrets Manager](https://github.com/SoftDryzz/vaultic)

*CLI for securely managing secrets and configuration across teams, with Git-based sync. Published on [crates.io](https://crates.io/crates/vaultic).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![crates.io](https://img.shields.io/crates/v/vaultic?style=flat-square&color=E6B14C)

- 🔒 **Strong encryption:** age or GPG with multi-recipient support, no external cloud
- 🌍 **Multi-environment:** dev/staging/prod with smart inheritance, diff and missing-variable detection
- 🚀 **CI/CD ready:** `vaultic ci export` for GitHub/GitLab, `VAULTIC_AGE_KEY`, `--stdout` piping and CI-friendly exit codes

<details>
<summary><b>More</b></summary>

- 📋 **Audit trail:** JSON history of who changed what and when
- 🏷️ 6 releases, latest v1.4.2

</details>

#### 🛡️ Cerberus v1.0: Security Monitor for Windows

*Real-time process, executable and network monitoring with threat detection. Also available as an extended **Pro** edition.*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- 🔴 **Process monitor:** real-time analysis with risk scoring (0-100)
- 🔵 **Executable analyzer:** hash verification, PE analysis, VirusTotal integration
- 🟢 **Network & system:** per-process connections, startup items and scheduled tasks

<details>
<summary><b>More</b></summary>

- 🟣 **Alerts & reports:** native notifications, PDF export, auto-updater
- 🧪 119 unit tests
- ⭐ **Cerberus Pro:** extended threat intelligence and professional features

</details>

#### 🛠️ [ProjectManager v2.1: CLI](https://github.com/SoftDryzz/ProjectManager)

*One command for all your projects. Detects the project type and standardizes build/run/test with diagnostics, security and statistics.*

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![Release](https://img.shields.io/github/v/release/SoftDryzz/ProjectManager?style=flat-square&color=2ea44f)

- 🔍 **Auto-detection:** 12+ project types (Gradle, Maven, Node.js, .NET, Python, Rust, Go, Flutter, Docker...)
- 🩺 **Diagnostics & security:** `pm doctor` with A-F scoring, `pm secure` and `pm audit`
- ✅ **800+ tests**, cross-platform (Windows, Linux, macOS), 30 releases

### 🦀 Open-Source Rust Crates

| Crate | What it does | Version |
|---|---|---|
| [**tower-rate-tier**](https://github.com/SoftDryzz/tower-rate-tier) | Tier-based rate limiting for Tower: per-plan limits (free/pro/enterprise), GCRA with per-request cost, in-memory (DashMap) or Redis storage, standard headers | [![crates.io](https://img.shields.io/crates/v/tower-rate-tier?style=flat-square&color=E6B14C)](https://crates.io/crates/tower-rate-tier) |
| [**tower-request-guard**](https://github.com/SoftDryzz/tower-request-guard) | One configurable guard instead of 3-4 layers: body size, per-route timeouts, Content-Type, required headers and JSON-bomb protection, with a dry-run `LogAndPass` mode | [![crates.io](https://img.shields.io/crates/v/tower-request-guard?style=flat-square&color=E6B14C)](https://crates.io/crates/tower-request-guard) |
| [**vaultic**](https://github.com/SoftDryzz/vaultic) | Secrets manager CLI (see above) | [![crates.io](https://img.shields.io/crates/v/vaultic?style=flat-square&color=E6B14C)](https://crates.io/crates/vaultic) |

Both Tower crates work with Axum, Hyper, Tonic and any Tower service.

### 🧾 Business Software

#### 🧾 VeriFactu E-Invoicing Application

*Self-hosted and desktop electronic invoicing for Spanish businesses, compliant with VeriFactu (AEAT, the Spanish tax agency).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/Axum-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![SvelteKit](https://img.shields.io/badge/SvelteKit-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- 🔗 **VeriFactu compliance:** chained invoice fingerprints, XML serialization and SOAP submission to the AEAT, verifiable QR codes
- 🧭 **Strict invoice lifecycle:** backend-owned state machine that only shows official AEAT states
- 🖥️ **Two deployments:** Axum server or Tauri desktop app, same SvelteKit UI

<details>
<summary><b>More</b></summary>

- 📋 Audit log and licensing server architecture
- 🧪 QA reports, test invoice suites and a penetration-test self-assessment
- 🔄 Self-hosted CI runner

</details>

#### 📈 Capital-Gains Tax Engine

*B2B engine that computes capital gains and losses on investments with the FIFO method for Spanish income tax (IRPF), built for tax advisors.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

#### ⚽ Sports Matchmaking Platform

*Mobile and web platform to organize matches, manage teams, track statistics, book pitches and run leagues and tournaments.*

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=firebase&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- 📱 Flutter app for iOS, Android and Web
- 🦀 Rust + Axum API (workspace with api, core, db and common crates)
- 🔔 Push notifications via Firebase (FCM + APNs)

### 🤖 AI & Automation

#### 🧠 Project Pandora: Self-Evolving Local AI Agent

*Autonomous AI agent that runs entirely on local hardware. 9 phases shipped.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- 🧩 **Four specialized LLM brains:** conversation, code, reasoning and fast tasks (Qwen3, DeepSeek-R1 via Ollama)
- 🔁 **Self-evolution engine:** prompts and tools improved through benchmarks
- 🛑 **6-level autonomy ladder** with an emergency kill switch

<details>
<summary><b>More</b></summary>

- 🛠️ **Integrated tools:** files, code generation, Docker sandbox and web scraping
- 🎙️ **Bilingual voice pipeline:** Whisper STT, Kokoro TTS and Silero VAD
- 🗂️ **Persistent memory:** episodic memory plus a ChromaDB vector store
- 🦀 Rust modules via PyO3

</details>

### 🧩 More Projects

| Project | What it is | Stack |
|---|---|---|
| **Vrydex** 🔒 | SaaS developer dashboard: GitHub repository health (outdated dependencies, vulnerabilities) plus Linux server monitoring, with GitHub OAuth | Rust |
| **MineHub** 🔒 | Local Minecraft server management hub: players, console, permissions, mods, modpacks, texture packs and datapacks | Rust |
| **Hyperions MC network** 🔒 | Cross-play Minecraft network infrastructure: Velocity proxy in front of Paper 1.21 servers, shared MariaDB, status page monitored from Cloudflare, Discord bots and website | Java · TypeScript · Python |
| **ProLoginAuth · ProSkins** 🔒 | Commercial Paper 1.21 plugins for cross-play servers: premium auto-login verified against Mojang, password auth for non-premium players, Bedrock via Floodgate, and skins for non-premium players | Java |
| **Spectra** 🔒 | Discord bot for development-team servers: channel management, daily standups, GitHub webhooks and onboarding | TypeScript |
| **xt** 🔒 | Terminal-art generator (graffiti and glitch logos drawn with half-block characters) plus a personal CLI that cross-checks GitHub repos against local clones | JavaScript |
| [FileSystemMonitor](https://github.com/SoftDryzz/FileSystemMonitor) | Real-time file system change monitor for Windows | C# · WPF |
| [WindowsOptimizer](https://github.com/SoftDryzz/WindowsOptimizer) | Cleanup, startup management and system tweaks for Windows | C# · .NET 8 |
| [system_monitor](https://github.com/SoftDryzz/system_monitor) | Cross-platform CLI system monitor with health indicators and watch mode | Rust |

🔒 Private repository

---

## ✍️ Latest from the Blog

| Post | Topic |
|---|---|
| [Ring -1: the hypervisor watching over your kernel](https://softdryzz.com/blog/posts/ring-menos-1-hipervisor) | Hypervisors, VT-x/AMD-V, EPT, VBS/HVCI · C++ `CPUID` examples |
| [From Ring 3 to Ring 0: what happens when your code crosses into the kernel](https://softdryzz.com/blog/posts/de-ring-3-a-ring-0) | Privilege rings, syscalls, kernel defenses · C++ examples |
| [Why Rust remains the safest language in 2026](https://softdryzz.com/blog/posts/rust-memory-safety-2026) | Ownership, borrowing and memory safety |

*Bilingual posts (ES/EN). The code in the Ring 0 / Ring -1 series is compiled and run on Linux and Windows before publishing.* → [All posts](https://softdryzz.com/blog/)

---

## 🛠️ Tech Stack

**Languages**

![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20asm-6E4C13?style=for-the-badge&logo=intel&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white)
![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Lua](https://img.shields.io/badge/lua-%232C2D72.svg?style=for-the-badge&logo=lua&logoColor=white)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=amazondocumentdb&logoColor=white)

**Systems & Reverse Engineering**

![Windows Driver Kit](https://img.shields.io/badge/WDK-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Intel VT-x](https://img.shields.io/badge/Intel%20VT--x-0071C5?style=for-the-badge&logo=intel&logoColor=white)
![Ghidra](https://img.shields.io/badge/Ghidra-D22128?style=for-the-badge&logoColor=white)
![x64dbg](https://img.shields.io/badge/x64dbg-2B2B2B?style=for-the-badge&logoColor=white)
![WinDbg](https://img.shields.io/badge/WinDbg-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![wgpu](https://img.shields.io/badge/wgpu%20%C2%B7%20WGSL-000000?style=for-the-badge&logo=rust&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

<details>
<summary><b>Backend, frontend, mobile, data & DevOps</b></summary>

**Backend & Runtime**

![Tokio](https://img.shields.io/badge/tokio-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/axum-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/tauri-%2324C8DB.svg?style=for-the-badge&logo=tauri&logoColor=%23FFFFFF)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Frontend & Mobile**

![Svelte](https://img.shields.io/badge/svelte-%23f1413d.svg?style=for-the-badge&logo=svelte&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)

**Data & DevOps**

![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

</details>

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
