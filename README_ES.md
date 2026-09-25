<div align="center">

**Desarrollador de Sistemas y Full-Stack · Rust · C++ · TypeScript · Fundador de [SoftDryzz](https://softdryzz.com)**

*Del Ring 0 al navegador: construyo hipervisores, herramientas de ingeniería inversa, software de seguridad, CLIs y plataformas web.*

[![Website](https://img.shields.io/badge/softdryzz.com-FF5722?style=flat-square&logo=google-chrome&logoColor=white)](https://softdryzz.com)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:contact@softdryzz.com)
[![Disponible](https://img.shields.io/badge/Disponible%20para%20proyectos-00C853?style=flat-square)](#-contáctame)

🌐 *[Read in English](README.md)*

</div>

---

## 🚀 Sobre Mí

- 🔬 **Bajo nivel primero:** Drivers de kernel de Windows, virtualización Intel VT-x e internals de x86-64. Me gusta saber qué está haciendo realmente la máquina.
- 🕵️ **Ingeniero inverso:** Análisis estático y dinámico de binarios, memoria de procesos y protocolos de red con Ghidra y x64dbg.
- 🔒 **Constructor de seguridad:** Detección de amenazas, monitorización de sistemas, gestión de secretos, licenciamiento y anti-manipulación.
- 🦀 **Backend y full-stack:** **Rust**, **C++**, **Java**, **TypeScript** y **Python**, desde middleware Tower hasta frontends React/Svelte y apps de escritorio con Tauri.
- 🤖 **IA y automatización:** Agentes de IA locales, integración de LLMs y automatización de procesos.

---

## 🧭 En Qué Trabajo

| Área | Qué abarca |
|---|---|
| 🔬 **Sistemas y Bajo Nivel** | Drivers de kernel de Windows (WDK), hipervisores Type-1 (VMX, EPT, VMCS, VM-exits), ensamblador x86-64, internals de Windows |
| 🕵️ **Ingeniería Inversa** | Ghidra, x64dbg, triaje de PE, unpacking, análisis anti-debug, análisis de memoria de procesos, reversing de protocolos de red |
| 🔒 **Herramientas de Seguridad** | Detección de amenazas, monitorización de sistemas, gestión de secretos, licenciamiento offline y anti-manipulación, hardening de servidores Linux |
| 🦀 **Backend y APIs** | Rust (Axum, Tower, Tokio), Java, Python (FastAPI), PostgreSQL, Redis |
| 🌐 **Frontend y Escritorio** | React, Next.js, Svelte, TailwindCSS, Tauri |
| 🎮 **Tooling y Modding de Juegos** | Plugins de servidor Minecraft (Paper/Velocity), addons de Meteor Client, análisis de memoria y protocolos de juegos |

---

## 📂 Proyectos Destacados

### 🔬 Sistemas e Ingeniería Inversa

#### 🌀 Hyperion: Hipervisor Type-1 para Windows

*Hipervisor Intel VT-x para Windows x64. Driver de kernel Ring 0 en C++ y loader Ring 3 en Rust, con introspección de máquina virtual y protección anti-reversing.*

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20ASM-6E4C13?style=flat-square&logo=intel&logoColor=white)
![WDK](https://img.shields.io/badge/WDK-0078D6?style=flat-square&logo=windows&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- ⚙️ **Núcleo VMX:** Configuración de VMCS, manejador de VM-exits, stubs en ensamblador x64 y emulación de CPUID
- 🧱 **Virtualización de memoria:** EPT, tablas de páginas shadow con copy-on-write, tipado según MTRR y batching diferido de INVEPT
- 🪝 **Hooking EPT y VMI:** Introspección con filtrado de VM-exits en kernel, trazado de rutas de ejecución y scoring de anomalías
- 🔌 **Telemetría Ring 0 → Ring 3:** Pipeline asíncrono con doble buffer, control de desbordamiento y gateway IOCTL, con loader en Rust
- 📊 **Rendimiento:** Profiling de latencia sub-microsegundo e histogramas de ejecución, anti-reversing multicapa
- 🧪 **Validación:** Despliegue en 5 fases con puertas de control y fire-tests

---

### 🔐 Seguridad y Herramientas para Desarrolladores

#### 🔐 [Vaultic v1.4: Gestor de Secretos](https://github.com/SoftDryzz/vaultic)

*CLI para gestionar secretos y configuración de forma segura entre equipos, con sincronización basada en Git. Publicada en [crates.io](https://crates.io/crates/vaultic).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)

- 🔒 **Cifrado robusto:** age o GPG con soporte multi-recipient, sin cloud externa
- 🌍 **Multi-entorno:** dev/staging/prod con herencia inteligente, diff y detección de variables ausentes
- 🚀 **Listo para CI/CD:** `vaultic ci export` para GitHub/GitLab, `VAULTIC_AGE_KEY`, salida por `--stdout` y códigos de salida pensados para CI
- 📋 **Registro de auditoría:** Historial JSON de quién cambió qué y cuándo

#### 🛡️ Cerberus v1.0: Monitor de Seguridad

*Monitor de seguridad privado para Windows con detección de amenazas en tiempo real.*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- 🔴 **Monitor de procesos:** Análisis en tiempo real con puntuación de riesgo (0-100)
- 🔵 **Analizador de ejecutables:** Verificación de hash, análisis PE, integración con VirusTotal
- 🟢 **Red y sistema:** Conexiones por proceso, programas de inicio y tareas programadas
- 🟣 **Alertas e informes:** Notificaciones nativas, exportación a PDF, auto-actualización, 119 unit tests

#### 🛠️ [ProjectManager v2.0: CLI](https://github.com/SoftDryzz/ProjectManager)

*Un comando para todos tus proyectos. Detecta el tipo y estandariza build/run/test con diagnósticos, seguridad y estadísticas.*

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)

- 🔍 **Detección automática:** 12+ tipos de proyecto (Gradle, Maven, Node.js, .NET, Python, Rust, Go, Flutter, Docker...)
- 🩺 **Diagnóstico y seguridad:** `pm doctor` con puntuación A-F, `pm secure` y `pm audit`
- ✅ **800+ tests:** Multiplataforma (Windows, Linux, macOS)

---

### 🦀 Crates de Rust

#### 🌐 [Tower Rate Tier v0.2](https://github.com/SoftDryzz/tower-rate-tier) · [crates.io](https://crates.io/crates/tower-rate-tier)

*Middleware de rate limiting por niveles para Tower. Límites por plan (free/pro/enterprise), coste por petición, storage intercambiable y headers estándar.*

- 📈 **Algoritmo GCRA** con coste por petición y ventanas diarias o personalizadas
- 🔌 **Storage intercambiable:** En memoria (DashMap) o Redis para múltiples servidores
- 🎛️ **Personalizable:** Callback `on_limited` y respuestas 429 a medida, benchmarks con Criterion
- 🏗️ **Nativo de Tower:** Axum, Hyper y cualquier servicio Tower, MSRV 1.75

#### 🧰 [Tower Request Guard v0.1](https://github.com/SoftDryzz/tower-request-guard) · [crates.io](https://crates.io/crates/tower-request-guard)

*Middleware de validación de peticiones para Tower. Sustituye 3-4 capas separadas por un único guard configurable.*

- 📏 **Validación:** Tamaño máximo de body, timeouts por ruta, Content-Type y headers obligatorios
- 💣 **Protección contra JSON bombs:** Validación de profundidad máxima de anidamiento
- 🧭 **Overrides por ruta** y modo `LogAndPass` (dry-run) para migraciones graduales
- 🏗️ **Nativo de Tower:** Axum, Tonic, Hyper o cualquier framework basado en Tower

---

## 🛠️ Stack Tecnológico

**Lenguajes**

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

**Sistemas e Ingeniería Inversa**

![Windows Driver Kit](https://img.shields.io/badge/WDK-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Intel VT-x](https://img.shields.io/badge/Intel%20VT--x-0071C5?style=for-the-badge&logo=intel&logoColor=white)
![Ghidra](https://img.shields.io/badge/Ghidra-D22128?style=for-the-badge&logoColor=white)
![x64dbg](https://img.shields.io/badge/x64dbg-2B2B2B?style=for-the-badge&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

**Backend y Runtime**

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

**Datos y DevOps**

![PostgreSQL](https://img.shields.io/badge/postgresql-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

---

## 💼 En Qué Puedo Ayudarte

Disponible para trabajos freelance y colaboraciones a través de [softdryzz.com](https://softdryzz.com):

| Servicio | Descripción |
|---|---|
| 🕵️ **Ingeniería Inversa** | Análisis de binarios y protocolos, revisión de protecciones de software, investigación de interoperabilidad |
| 🔬 **Desarrollo de Bajo Nivel** | Drivers de Windows, virtualización, Rust/C++ de alto rendimiento |
| 🔒 **Seguridad y Hardening** | Herramientas de monitorización y detección, gestión de secretos, hardening de servidores |
| 💻 **Software a Medida** | Apps de escritorio, CLIs, APIs, middleware e integraciones |
| 🌐 **Desarrollo Web** | Landing pages, plataformas web, e-commerce |
| 🧠 **Consultoría Digital e IA** | Planes de digitalización, integración de IA, automatización de procesos |

---

## 🎓 Formación y Certificaciones

| Título | Institución |
|---|---|
| **Desarrollo de Aplicaciones Multiplataforma (DAM)** | Campus Cámara de Comercio de Sevilla |
| **Digitalización de Empresas** | EOI (Escuela de Organización Industrial) |
| **Especialista en Inteligencia Artificial** | Founderz |

---

## 📈 Estadísticas de GitHub

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

## 📫 Contáctame

[![Website](https://img.shields.io/badge/Website-softdryzz.com-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://softdryzz.com)

| | Email | Uso |
|---|---|---|
| 📩 | **contact@softdryzz.com** | Consultas generales y colaboraciones |
| 🛡️ | **security@softdryzz.com** | Vulnerabilidades de seguridad y divulgación responsable |
| ⚖️ | **legal@softdryzz.com** | Licencias comerciales |
| 👤 | **cristo@softdryzz.com** | Contacto directo |

---

<p align="center">
  <a href="https://github.com/sponsors/SoftDryzz">
    <img src="https://img.shields.io/badge/Sponsor-💗-ea4aaa?style=for-the-badge&logo=github" height="40" alt="GitHub Sponsors">
  </a>
  &nbsp;&nbsp;
  <a href="https://buymeacoffee.com/xtoftomeo" target="_blank">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="40" alt="Invítame a un Café">
  </a>
</p>

<p align="center"><i>"El código es como el humor. Cuando tienes que explicarlo, es malo." · Cory House</i></p>

<p align="center"><b>¡Construyamos algo increíble juntos!</b> 🚀</p>
