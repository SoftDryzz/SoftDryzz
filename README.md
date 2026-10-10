<div align="center">

## Cristo Fernández Tomé

**AI trainer for business · Software, systems, servers & AI engineering**

*From the operating system kernel to AI agents. I teach the AI I build.*

[![Website](https://img.shields.io/badge/softdryzz.com-FF5722?style=flat-square&logo=google-chrome&logoColor=white)](https://softdryzz.com)
[![Blog](https://img.shields.io/badge/Blog-111111?style=flat-square&logo=rss&logoColor=white)](https://softdryzz.com/blog/)
[![crates.io](https://img.shields.io/badge/crates.io-3%20crates-E6B14C?style=flat-square&logo=rust&logoColor=white)](https://crates.io/crates/vaultic)
[![Email](https://img.shields.io/badge/xtoftome@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:xtoftome@gmail.com)
[![Available](https://img.shields.io/badge/Available%20for%20training%20%26%20projects-00C853?style=flat-square)](#-contact)

🌐 *[Leer en Español](README_ES.md)*

</div>

---

## 🎯 What I Do

| | |
|---|---|
| 🎓 **AI training** | Applied AI training for companies and institutions · **300+ hours** delivered · **50+ people** trained · **6+ sectors** |
| 🏢 **AXIOM ZERO S.L.** | Founder, CEO & CTO (company in incorporation) |
| 🧪 **R&D leadership** | R&D Director at an industrial company in the olive oil sector |
| 🤖 **AI consulting** | AI consulting and automation through [SoftDryzz](https://softdryzz.com) |

---

## 🧠 Flagship Project: Pandora

*My own autonomous, self-evolving AI system, running 100% locally. 21K+ lines of code. Private code, demo on request.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Demo on request](https://img.shields.io/badge/private%20code-demo%20on%20request-555555?style=flat-square&logo=github)

- 🧩 **Multi-model orchestration:** 4 specialized models on Ollama (conversation, code, reasoning and fast tasks)
- 🗂️ **Long-term memory:** RAG, episodic memory and a knowledge graph
- 🔁 **Self-optimization:** improves its own prompts and tools by measuring itself against benchmarks
- 🎙️ **Bilingual voice:** Whisper STT, Kokoro TTS and Silero VAD
- 🛑 **Governance:** 6 autonomy levels and an emergency kill switch

---

## 🧭 Engineering Areas

| Area | What it covers |
|---|---|
| 🤖 **Applied AI** | AI systems and agents, local models with Ollama, RAG, voice, process automation |
| 🖥️ **Servers & infrastructure** | 25+ servers (VPS, dedicated and Windows Server) · automated hardening (SSH keys, UFW, Fail2Ban, AppArmor, auditd, AIDE, Lynis) · CI/CD with Docker and GitHub Actions · backups, monitoring and alerts · VPN and Cloudflare |
| 📋 **ISO standards** | Experience with ISO/IEC 27001, ISO/IEC 42001, ISO 9001, ISO 14001 and ISO 22000 (with IFS/BRC) management systems |
| 🔒 **Cybersecurity** | Threat monitoring and detection, secrets management, coordinated vulnerability disclosure (GHSA) |
| 🔬 **Systems & low-level** | Windows kernel drivers (WDK), Type-1 hypervisors (VMX, EPT, VMCS, VM-exits), x86-64 assembly, Windows internals |
| 🕵️ **Reverse engineering (security research)** | Ghidra, x64dbg, WinDbg · PE executable triage and analysis in an isolated lab |
| 🧾 **Regulated business software** | Spanish e-invoicing (VeriFactu / AEAT), tax calculation engines, audit trails |
| 🦀 **Backend, frontend & mobile** | Rust (Axum, Tower, Tokio), Java, Python (FastAPI), PostgreSQL, Redis · React, Next.js, SvelteKit, Tauri, Flutter |

## 🔭 Right Now

- 🎓 Delivering **applied AI training** for companies and institutions
- 🧾 Building a **VeriFactu-compliant e-invoicing application** (Rust · Axum · Tauri · SvelteKit) and a **capital-gains tax engine** (FIFO / Spanish IRPF) for tax advisors
- 🦀 Shipped [tower-rate-tier v0.3.0](https://github.com/SoftDryzz/tower-rate-tier/releases/tag/v0.3.0): rate limits shared across instances through Redis, with a [walkthrough on the blog](https://softdryzz.com/blog/posts/tower-rate-tier-limitar-por-plan) (October 2026)
- 🔐 Shipped [Vaultic v1.4.3](https://github.com/SoftDryzz/vaultic/releases/tag/v1.4.3), a security release with a [public post-mortem](https://softdryzz.com/blog/posts/vaultic-secreto-que-ejecutaba-codigo) (September 2026)

---

## 📂 Featured Projects

### 🔬 Systems & Security Research

#### 🌀 Hyperion: Custom hypervisor (Intel VT-x/EPT)

*Type-1 hypervisor for Windows x64: Ring 0 kernel driver in C++ plus a Ring 3 loader in Rust, with virtual machine introspection (VMI) and anomaly detection.*

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20ASM-6E4C13?style=flat-square&logo=intel&logoColor=white)
![WDK](https://img.shields.io/badge/WDK-0078D6?style=flat-square&logo=windows&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

- ⚙️ **VMX core:** VMCS setup, VM-exit handler, x64 assembly entry stubs and CPUID emulation
- 🧱 **Memory virtualization:** EPT with MTRR-aware memory typing, deferred INVEPT batching and copy-on-write shadow page tables
- 🔎 **Introspection & telemetry:** VM-exit filtering, execution path tracing and anomaly scoring, with a Ring 0 → Ring 3 pipeline over IOCTL

<details>
<summary><b>More internals</b></summary>

- 📊 Sub-microsecond latency profiling and execution histograms
- 🧪 5-phase gated deployment, tested under nested virtualization

</details>

### 🔐 Security & Developer Tools

#### 🔐 [Vaultic v1.4.3: Secrets Manager](https://github.com/SoftDryzz/vaultic)

*CLI for securely managing secrets and configuration across teams, with Git-based sync. Published on [crates.io](https://crates.io/crates/vaultic).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![crates.io](https://img.shields.io/crates/v/vaultic?style=flat-square&color=E6B14C)

- 🔒 **Strong encryption:** age or GPG with multi-recipient support, no external cloud
- 🌍 **Multi-environment:** dev/staging/prod with smart inheritance, diff and missing-variable detection
- 🚀 **CI/CD ready:** `vaultic ci export` for GitHub/GitLab, `--stdout` piping and CI-friendly exit codes

<details>
<summary><b>More</b></summary>

- 🛡️ **Security release v1.4.3:** fixed a high-severity command injection in `ci export` ([GHSA-5cfx-fmm5-7p2f](https://github.com/SoftDryzz/vaultic/security/advisories/GHSA-5cfx-fmm5-7p2f)), owner-only permissions for keys and decrypted files, atomic writes · [post-mortem](https://softdryzz.com/blog/posts/vaultic-secreto-que-ejecutaba-codigo)
- 📋 **Audit trail:** JSON history of who changed what and when
- 🏷️ 7 releases, latest v1.4.3

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
- 🟢 **Network & system:** per-process connections, startup items and scheduled tasks · native alerts, PDF reports and 119 unit tests

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
| [**tower-rate-tier**](https://github.com/SoftDryzz/tower-rate-tier) | Tier-based rate limiting for Tower: per-plan limits (free/pro/enterprise), GCRA with per-request cost, limits shared across instances through Redis or in-memory (DashMap), safe defaults for unknown plans, standard headers · [walkthrough](https://softdryzz.com/blog/posts/tower-rate-tier-limitar-por-plan) | [![crates.io](https://img.shields.io/crates/v/tower-rate-tier?style=flat-square&color=E6B14C)](https://crates.io/crates/tower-rate-tier) |
| [**tower-request-guard**](https://github.com/SoftDryzz/tower-request-guard) | One configurable guard instead of 3-4 layers: body size, per-route timeouts, Content-Type, required headers and JSON-bomb protection, with a dry-run `LogAndPass` mode | [![crates.io](https://img.shields.io/crates/v/tower-request-guard?style=flat-square&color=E6B14C)](https://crates.io/crates/tower-request-guard) |
| [**vaultic**](https://github.com/SoftDryzz/vaultic) | Secrets manager CLI (see above) | [![crates.io](https://img.shields.io/crates/v/vaultic?style=flat-square&color=E6B14C)](https://crates.io/crates/vaultic) |

Both Tower crates work with Axum, Hyper and other Tower services; tower-request-guard also works with Tonic (Tonic support in tower-rate-tier is planned). 40+ public releases on GitHub in total.

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
- 🖥️ **Two deployments:** Axum server or Tauri desktop app, same SvelteKit UI · audit log, test invoice suites and a penetration-test self-assessment

#### 📈 Capital-Gains Tax Engine

*B2B engine that computes capital gains and losses on investments with the FIFO method for Spanish income tax (IRPF), built for tax advisors.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

#### ⚽ Sports Matchmaking Platform

*Mobile and web platform to organize matches, manage teams, track statistics, book pitches and run leagues and tournaments. Flutter app (iOS, Android and Web), Rust + Axum API and Firebase push notifications.*

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=firebase&logoColor=white)
![Private](https://img.shields.io/badge/repo-private-555555?style=flat-square&logo=github)

### 🧩 More Projects

| Project | What it is | Stack |
|---|---|---|
| **CXC** 🔒 | Crawler that indexes code for AI agents (RAG/MCP integration planned) | Rust |
| **Vrydex** 🔒 | SaaS developer dashboard: GitHub repository health (outdated dependencies, vulnerabilities) plus Linux server monitoring, with GitHub OAuth | Rust |
| **Spectra** 🔒 | Discord bot for development-team servers: channel management, daily standups, GitHub webhooks and onboarding | TypeScript |
| [FileSystemMonitor](https://github.com/SoftDryzz/FileSystemMonitor) | Real-time file system change monitor for Windows | C# · WPF |
| [WindowsOptimizer](https://github.com/SoftDryzz/WindowsOptimizer) | Cleanup, startup management and system tweaks for Windows | C# · .NET 8 |
| [system_monitor](https://github.com/SoftDryzz/system_monitor) | Cross-platform CLI system monitor with health indicators and watch mode | Rust |

🔒 Private repository

---

## ✍️ Latest from the Blog

| Post | Topic |
|---|---|
| [Rate limiting an API by plan in Rust: GCRA, Redis and tower-rate-tier](https://softdryzz.com/blog/posts/tower-rate-tier-limitar-por-plan) | Per-plan limits, why GCRA instead of a fixed window, requests that cost more, limits shared across instances with Redis, safe defaults · example service with real output |
| [Using C++ from Rust: how a safe wrapper turns a use-after-free into a compile error](https://softdryzz.com/blog/posts/rust-cpp-ffi-unsafe) | `unsafe` and its five superpowers, a C API over C++, `#[repr(C)]`, lifetimes that encode a C++ contract, `Send`/`Sync`, panics across `extern "C"` · Rust + C++ code |
| [A secret that ran code: post-mortem of a vulnerability in my own secrets manager](https://softdryzz.com/blog/posts/vaultic-secreto-que-ejecutaba-codigo) | Command injection through `eval` in CI, single-quote escaping, newlines in `$GITHUB_ENV`, coordinated disclosure (GHSA) |
| [Anatomy of a Windows driver: from DriverEntry to the IRP](https://softdryzz.com/blog/posts/anatomia-driver-windows) | `DriverEntry`, IRQL, the journey of an IRP, dispatch table, custom IOCTLs, spinlocks · C++ code |
| [x86 privilege rings: from Ring 3 to Ring -2](https://softdryzz.com/blog/series/anillos-x86) (complete series) | [Ring 0](https://softdryzz.com/blog/posts/de-ring-3-a-ring-0): syscalls and kernel defenses → [Ring -1](https://softdryzz.com/blog/posts/ring-menos-1-hipervisor): VT-x, EPT, VBS/HVCI → [Ring -2](https://softdryzz.com/blog/posts/ring-menos-2-smm): SMM, SMRAM, WSMT · C++ examples |
| [Why Rust remains the safest language in 2026](https://softdryzz.com/blog/posts/rust-memory-safety-2026) | Ownership, borrowing and memory safety |

*Bilingual posts (ES/EN). The code in the [x86 privilege rings series](https://softdryzz.com/blog/series/anillos-x86) is compiled and run before publishing.* → [All posts](https://softdryzz.com/blog/) · [RSS](https://softdryzz.com/blog/feed-en.xml)

---

## 🛠️ Tech Stack

**Languages**

![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20asm-6E4C13?style=for-the-badge&logo=intel&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white)
![Dart](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=amazondocumentdb&logoColor=white)

**AI, Servers & DevOps**

![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white)

**Systems & Reverse Engineering**

![Windows Driver Kit](https://img.shields.io/badge/WDK-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Intel VT-x](https://img.shields.io/badge/Intel%20VT--x-0071C5?style=for-the-badge&logo=intel&logoColor=white)
![Ghidra](https://img.shields.io/badge/Ghidra-D22128?style=for-the-badge&logoColor=white)
![x64dbg](https://img.shields.io/badge/x64dbg-2B2B2B?style=for-the-badge&logoColor=white)
![WinDbg](https://img.shields.io/badge/WinDbg-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

<details>
<summary><b>Backend, frontend, mobile & data</b></summary>

**Backend & Runtime**

![Tokio](https://img.shields.io/badge/tokio-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/axum-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/tauri-%2324C8DB.svg?style=for-the-badge&logo=tauri&logoColor=%23FFFFFF)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)

**Frontend & Mobile**

![Svelte](https://img.shields.io/badge/svelte-%23f1413d.svg?style=for-the-badge&logo=svelte&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)

**Data**

![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

</details>

---

## 💼 What I Can Help With

| Service | Description |
|---|---|
| 🎓 **AI training** | Applied AI training for companies and institutions, tailored to each team |
| 🧠 **AI consulting & automation** | Digitalization plans, AI integration, local AI and process automation |
| 🖥️ **Servers & infrastructure** | Server deployment and administration, hardening, CI/CD, backups and monitoring |
| 🔒 **Cybersecurity & ISO standards** | Monitoring and detection tooling, secrets management, ISO/IEC 27001 and 42001 management systems |
| 💻 **Custom software** | Desktop apps, CLIs, APIs, web platforms and integrations |
| 🔬 **Low-level & security research** | Windows drivers, virtualization, binary analysis, performance-critical Rust/C++ |

---

## 📈 GitHub Stats

<p align="center">
  <img src="./profile/stats.svg" height="165" alt="GitHub stats" />
  <img src="./profile/top-langs.svg" height="165" alt="Top languages" />
</p>

<p align="center">
  <img src="./profile-3d-contrib/profile-night-rainbow.svg" alt="3D contribution graph" />
</p>

---

## 📫 Contact

| | |
|---|---|
| 📩 **Email** | [xtoftome@gmail.com](mailto:xtoftome@gmail.com) |
| 🌐 **Website & blog** | [softdryzz.com](https://softdryzz.com) · [softdryzz.com/blog](https://softdryzz.com/blog/) |
| 🛡️ **Security** | security@softdryzz.com · responsible vulnerability disclosure |
