<div align="center">


**Desarrollador de Sistemas y Full-Stack · C++ · Rust · TypeScript · Fundador de [SoftDryzz](https://softdryzz.com)**

*Del Ring 0 al navegador: construyo hipervisores, herramientas de ingeniería inversa, software de seguridad, CLIs y plataformas web.*

[![Web](https://img.shields.io/badge/softdryzz.com-FF5722?style=flat-square&logo=google-chrome&logoColor=white)](https://softdryzz.com)
[![Blog](https://img.shields.io/badge/Blog-111111?style=flat-square&logo=rss&logoColor=white)](https://softdryzz.com/blog/)
[![crates.io](https://img.shields.io/badge/crates.io-3%20crates-E6B14C?style=flat-square&logo=rust&logoColor=white)](https://crates.io/crates/vaultic)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:contact@softdryzz.com)
[![Disponible](https://img.shields.io/badge/Disponible%20para%20proyectos-00C853?style=flat-square)](#-contáctame)

🌐 *[Read in English](README.md)*

</div>

---

## ⚡ De un Vistazo

| | |
|---|---|
| 🔬 **Bajo nivel** | Drivers de kernel de Windows (WDK) · hipervisor Type-1 sobre Intel VT-x/EPT · ensamblador x86-64 |
| 🕵️ **Ingeniería inversa** | Ghidra · x64dbg · WinDbg · triaje de PE · laboratorio de análisis aislado |
| 🦀 **Open source** | 3 crates en crates.io · 40 releases públicas · 800+ tests en ProjectManager |
| 🧾 **Software de negocio** | Facturación electrónica VeriFactu y motor de plusvalías FIFO/IRPF para el mercado español |
| 📦 **Portfolio** | 50+ repositorios · lenguajes principales por volumen: C++, Java, Rust, TypeScript |

## 🔭 Ahora Mismo

- 🧾 Desarrollando una **aplicación de facturación electrónica compatible con VeriFactu** (Rust · Axum · Tauri · SvelteKit)
- 📈 Desarrollando un **motor de plusvalías** (FIFO / IRPF) para asesores fiscales
- ✍️ Escribiendo una serie en el blog sobre los anillos de privilegio de x86: [Ring 0](https://softdryzz.com/blog/posts/de-ring-3-a-ring-0) → [Ring -1](https://softdryzz.com/blog/posts/ring-menos-1-hipervisor) → Ring -2 (SMM) próximamente
- 🛠️ Publicada [ProjectManager v2.1](https://github.com/SoftDryzz/ProjectManager/releases) (septiembre de 2026)

---

## 🧭 En Qué Trabajo

| Área | Qué abarca |
|---|---|
| 🔬 **Sistemas y Bajo Nivel** | Drivers de kernel de Windows (WDK), hipervisores Type-1 (VMX, EPT, VMCS, VM-exits), ensamblador x86-64, internals de Windows |
| 🕵️ **Ingeniería Inversa** | Ghidra, x64dbg, WinDbg, triaje de PE, desempaquetado, análisis anti-debug, análisis de memoria de procesos, reversing de protocolos de red |
| 🔒 **Herramientas de Seguridad** | Detección de amenazas, monitorización del sistema, gestión de secretos, licencias offline y anti-tamper, hardening de servidores Linux |
| 🧾 **Software de Negocio Regulado** | Facturación electrónica española (VeriFactu / AEAT), motores de cálculo fiscal, registros de auditoría |
| 🦀 **Backend y APIs** | Rust (Axum, Tower, Tokio), Java, Python (FastAPI), PostgreSQL, Redis |
| 🌐 **Frontend, Escritorio y Móvil** | React, Next.js, Svelte/SvelteKit, TailwindCSS, Tauri, Flutter |
| 🎮 **Tooling y Modding de Juegos** | Plugins de servidor Minecraft (Paper/Velocity), addons de Meteor Client, análisis de memoria y protocolos de juegos |

---

## 📂 Proyectos Destacados

### 🔬 Sistemas e Ingeniería Inversa

#### 🌀 Hyperion: Hipervisor Type-1 para Windows

*Hipervisor sobre Intel VT-x para Windows x64. Driver de kernel en C++ (Ring 0) y loader en Rust (Ring 3), con introspección de VM y protección anti-reversing.*

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Assembly](https://img.shields.io/badge/x86--64%20ASM-6E4C13?style=flat-square&logo=intel&logoColor=white)
![WDK](https://img.shields.io/badge/WDK-0078D6?style=flat-square&logo=windows&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- ⚙️ **Núcleo VMX:** configuración de la VMCS, manejador de VM-exits, stubs de entrada en ensamblador x64 y emulación de CPUID
- 🧱 **Virtualización de memoria:** EPT con tipado de memoria según las MTRR y agrupación diferida de INVEPT
- 🔌 **Telemetría Ring 0 → Ring 3:** pipeline asíncrono de doble buffer sobre una pasarela IOCTL, loader en Rust

<details>
<summary><b>Más detalles internos</b></summary>

- 🧱 Tablas de páginas sombra con copy-on-write y split paging a 4 KB
- 🪝 **EPT hooking y VMI:** filtrado de VM-exits en el kernel, trazado de rutas de ejecución y puntuación de anomalías
- 📊 **Rendimiento:** perfilado de latencia por debajo del microsegundo e histogramas de ejecución, anti-reversing multicapa
- 🧪 **Validación:** despliegue por fases (5) con pruebas de fuego, probado con virtualización anidada

</details>

### 🔐 Seguridad y Herramientas para Desarrolladores

#### 🔐 [Vaultic v1.4: Gestor de Secretos](https://github.com/SoftDryzz/vaultic)

*CLI para gestionar secretos y configuración de forma segura en equipos, con sincronización vía Git. Publicado en [crates.io](https://crates.io/crates/vaultic).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![crates.io](https://img.shields.io/crates/v/vaultic?style=flat-square&color=E6B14C)

- 🔒 **Cifrado fuerte:** age o GPG con varios destinatarios, sin nube externa
- 🌍 **Multi-entorno:** dev/staging/prod con herencia inteligente, diff y detección de variables que faltan
- 🚀 **Listo para CI/CD:** `vaultic ci export` para GitHub/GitLab, `VAULTIC_AGE_KEY`, salida por `--stdout` y códigos de salida pensados para CI

<details>
<summary><b>Más</b></summary>

- 📋 **Auditoría:** historial JSON de quién cambió qué y cuándo
- 🏷️ 6 releases, la última v1.4.2

</details>

#### 🛡️ Cerberus v1.0: Monitor de Seguridad para Windows

*Monitorización en tiempo real de procesos, ejecutables y red con detección de amenazas. También existe una edición **Pro** ampliada.*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- 🔴 **Monitor de procesos:** análisis en tiempo real con puntuación de riesgo (0-100)
- 🔵 **Analizador de ejecutables:** verificación de hashes, análisis PE, integración con VirusTotal
- 🟢 **Red y sistema:** conexiones por proceso, elementos de inicio y tareas programadas

<details>
<summary><b>Más</b></summary>

- 🟣 **Alertas e informes:** notificaciones nativas, exportación a PDF, actualizador automático
- 🧪 119 tests unitarios
- ⭐ **Cerberus Pro:** inteligencia de amenazas ampliada y funciones profesionales

</details>

#### 🛠️ [ProjectManager v2.1: CLI](https://github.com/SoftDryzz/ProjectManager)

*Un solo comando para todos tus proyectos. Detecta el tipo de proyecto y unifica build/run/test con diagnóstico, seguridad y estadísticas.*

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![Release](https://img.shields.io/github/v/release/SoftDryzz/ProjectManager?style=flat-square&color=2ea44f)

- 🔍 **Autodetección:** 12+ tipos de proyecto (Gradle, Maven, Node.js, .NET, Python, Rust, Go, Flutter, Docker...)
- 🩺 **Diagnóstico y seguridad:** `pm doctor` con nota A-F, `pm secure` y `pm audit`
- ✅ **800+ tests**, multiplataforma (Windows, Linux, macOS), 30 releases

### 🦀 Crates de Rust Open Source

| Crate | Qué hace | Versión |
|---|---|---|
| [**tower-rate-tier**](https://github.com/SoftDryzz/tower-rate-tier) | Rate limiting por niveles para Tower: límites por plan (free/pro/enterprise), GCRA con coste por petición, almacenamiento en memoria (DashMap) o Redis, cabeceras estándar | [![crates.io](https://img.shields.io/crates/v/tower-rate-tier?style=flat-square&color=E6B14C)](https://crates.io/crates/tower-rate-tier) |
| [**tower-request-guard**](https://github.com/SoftDryzz/tower-request-guard) | Un guard configurable en lugar de 3-4 capas: tamaño de body, timeouts por ruta, Content-Type, cabeceras obligatorias y protección contra JSON bombs, con modo `LogAndPass` (dry-run) | [![crates.io](https://img.shields.io/crates/v/tower-request-guard?style=flat-square&color=E6B14C)](https://crates.io/crates/tower-request-guard) |
| [**vaultic**](https://github.com/SoftDryzz/vaultic) | CLI de gestión de secretos (ver arriba) | [![crates.io](https://img.shields.io/crates/v/vaultic?style=flat-square&color=E6B14C)](https://crates.io/crates/vaultic) |

Los dos crates de Tower funcionan con Axum, Hyper, Tonic y cualquier servicio Tower.

### 🧾 Software de Negocio

#### 🧾 Aplicación de Facturación Electrónica VeriFactu

*Facturación electrónica para empresas españolas, autoalojada o de escritorio, compatible con VeriFactu (AEAT).*

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/Axum-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![SvelteKit](https://img.shields.io/badge/SvelteKit-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- 🔗 **Cumplimiento VeriFactu:** huellas encadenadas de cada factura, serialización XML y envío SOAP a la AEAT, códigos QR verificables
- 🧭 **Ciclo de vida estricto:** máquina de estados en el backend que solo muestra los estados oficiales de la AEAT
- 🖥️ **Dos despliegues:** servidor Axum o app de escritorio Tauri, con la misma interfaz SvelteKit

<details>
<summary><b>Más</b></summary>

- 📋 Registro de auditoría y arquitectura de servidor de licencias
- 🧪 Informes de QA, baterías de facturas de prueba y autoevaluación de pentest
- 🔄 Runner de CI autoalojado

</details>

#### 📈 Motor de Plusvalías

*Motor B2B que calcula ganancias y pérdidas patrimoniales de inversiones con el método FIFO para el IRPF, pensado para asesores fiscales.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

#### ⚽ Plataforma para Organizar Partidos

*Plataforma móvil y web para organizar partidos, gestionar equipos, registrar estadísticas, reservar campos y participar en ligas y torneos.*

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=firebase&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- 📱 App Flutter para iOS, Android y Web
- 🦀 API en Rust + Axum (workspace con los crates api, core, db y common)
- 🔔 Notificaciones push con Firebase (FCM + APNs)

### 🤖 IA y Automatización

#### 🧠 Project Pandora: Agente de IA Local Auto-Evolutivo

*Agente de IA autónomo que se ejecuta íntegramente en hardware local. 9 fases completadas.*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Privado](https://img.shields.io/badge/repo-privado-555555?style=flat-square&logo=github)

- 🧩 **Cuatro cerebros LLM especializados:** conversación, código, razonamiento y tareas rápidas (Qwen3, DeepSeek-R1 vía Ollama)
- 🔁 **Motor de auto-evolución:** prompts y herramientas que mejoran mediante benchmarks
- 🛑 **6 niveles de autonomía** con kill switch de emergencia

<details>
<summary><b>Más</b></summary>

- 🛠️ **Herramientas integradas:** archivos, generación de código, sandbox Docker y web scraping
- 🎙️ **Pipeline de voz bilingüe:** Whisper STT, Kokoro TTS y Silero VAD
- 🗂️ **Memoria persistente:** memoria episódica y base vectorial ChromaDB
- 🦀 Módulos en Rust vía PyO3

</details>

### 🧩 Más Proyectos

| Proyecto | Qué es | Stack |
|---|---|---|
| **Vrydex** 🔒 | Panel SaaS para desarrolladores: salud de repositorios de GitHub (dependencias desactualizadas, vulnerabilidades) y monitorización de servidores Linux, con OAuth de GitHub | Rust |
| **MineHub** 🔒 | Centro de gestión local de servidores de Minecraft: jugadores, consola, permisos, mods, modpacks, texture packs y datapacks | Rust |
| **Red Hyperions MC** 🔒 | Infraestructura de una red de Minecraft cross-play: proxy Velocity delante de servidores Paper 1.21, MariaDB compartida, página de estado monitorizada desde Cloudflare, bots de Discord y web | Java · TypeScript · Python |
| **ProLoginAuth · ProSkins** 🔒 | Plugins comerciales para Paper 1.21 en servidores cross-play: auto-login premium verificado contra Mojang, contraseña para jugadores no premium, Bedrock vía Floodgate y skins para jugadores no premium | Java |
| **Spectra** 🔒 | Bot de Discord para servidores de equipos de desarrollo: gestión de canales, daily standups, webhooks de GitHub y onboarding | TypeScript |
| **xt** 🔒 | Generador de arte de terminal (logotipos grafiti y glitch con caracteres de medio bloque) y CLI personal que cruza los repos de GitHub con los clones locales | JavaScript |
| [FileSystemMonitor](https://github.com/SoftDryzz/FileSystemMonitor) | Monitor en tiempo real de cambios en el sistema de archivos de Windows | C# · WPF |
| [WindowsOptimizer](https://github.com/SoftDryzz/WindowsOptimizer) | Limpieza, gestión del arranque y ajustes del sistema para Windows | C# · .NET 8 |
| [system_monitor](https://github.com/SoftDryzz/system_monitor) | Monitor de sistema CLI multiplataforma con indicadores de salud y modo watch | Rust |

🔒 Repositorio privado

---

## ✍️ Últimas Entradas del Blog

| Entrada | Tema |
|---|---|
| [Ring -1: el hipervisor que vigila a tu kernel](https://softdryzz.com/blog/posts/ring-menos-1-hipervisor) | Hipervisores, VT-x/AMD-V, EPT, VBS/HVCI · ejemplos en C++ con `CPUID` |
| [De Ring 3 a Ring 0: qué pasa cuando tu código cruza la frontera del kernel](https://softdryzz.com/blog/posts/de-ring-3-a-ring-0) | Anillos de privilegio, syscalls, defensas del kernel · ejemplos en C++ |
| [Por qué Rust sigue siendo el lenguaje más seguro en 2026](https://softdryzz.com/blog/posts/rust-memory-safety-2026) | Ownership, borrowing y seguridad de memoria |

*Entradas bilingües (ES/EN). El código de la serie Ring 0 / Ring -1 se compila y ejecuta en Linux y Windows antes de publicarse.* → [Todas las entradas](https://softdryzz.com/blog/)

---

## 🛠️ Stack Tecnológico

**Lenguajes**

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

**Sistemas e Ingeniería Inversa**

![Windows Driver Kit](https://img.shields.io/badge/WDK-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Intel VT-x](https://img.shields.io/badge/Intel%20VT--x-0071C5?style=for-the-badge&logo=intel&logoColor=white)
![Ghidra](https://img.shields.io/badge/Ghidra-D22128?style=for-the-badge&logoColor=white)
![x64dbg](https://img.shields.io/badge/x64dbg-2B2B2B?style=for-the-badge&logoColor=white)
![WinDbg](https://img.shields.io/badge/WinDbg-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![wgpu](https://img.shields.io/badge/wgpu%20%C2%B7%20WGSL-000000?style=for-the-badge&logo=rust&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-064F8C?style=for-the-badge&logo=cmake&logoColor=white)

<details>
<summary><b>Backend, frontend, móvil, datos y DevOps</b></summary>

**Backend y Runtime**

![Tokio](https://img.shields.io/badge/tokio-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Axum](https://img.shields.io/badge/axum-%23000000.svg?style=for-the-badge&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/tauri-%2324C8DB.svg?style=for-the-badge&logo=tauri&logoColor=%23FFFFFF)
![Node.js](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)

**Frontend y Móvil**

![Svelte](https://img.shields.io/badge/svelte-%23f1413d.svg?style=for-the-badge&logo=svelte&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next.js](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)

**Datos y DevOps**

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

## 💼 En Qué Puedo Ayudarte

Disponible para trabajo freelance y colaboraciones a través de [softdryzz.com](https://softdryzz.com):

| Servicio | Descripción |
|---|---|
| 🕵️ **Ingeniería Inversa** | Análisis de binarios y protocolos, revisión de protecciones de software, investigación de interoperabilidad |
| 🔬 **Desarrollo de Bajo Nivel** | Drivers de Windows, virtualización, Rust/C++ de alto rendimiento |
| 🔒 **Herramientas de Seguridad y Hardening** | Herramientas de monitorización y detección, gestión de secretos, hardening de servidores |
| 💻 **Software a Medida** | Apps de escritorio, CLIs, APIs, middleware e integraciones |
| 🌐 **Desarrollo Web** | Landing pages, plataformas web, e-commerce |
| 🧠 **Consultoría Digital e IA** | Planes de digitalización, integración de IA, automatización de procesos |

---

## 📈 Estadísticas de GitHub

<p align="center">
  <img src="./profile/stats.svg" height="165" alt="Estadísticas de GitHub" />
  <img src="./profile/top-langs.svg" height="165" alt="Lenguajes principales" />
</p>

<p align="center">
  <img src="./profile-3d-contrib/profile-night-rainbow.svg" alt="Gráfico 3D de contribuciones" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=SoftDryzz&color=2ea44f&style=flat&label=Visitas+al+perfil" alt="Visitas al perfil" />
</p>

---

## 📫 Contáctame

[![Web](https://img.shields.io/badge/Web-softdryzz.com-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://softdryzz.com)

| | Email | Para qué |
|---|---|---|
| 📩 | **contact@softdryzz.com** | Consultas generales y colaboraciones |
| 🛡️ | **security@softdryzz.com** | Vulnerabilidades y divulgación responsable |
| ⚖️ | **legal@softdryzz.com** | Licencias comerciales |
| 👤 | **cristo@softdryzz.com** | Contacto directo |

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

<p align="center"><i>"El código es como el humor. Cuando tienes que explicarlo, es malo." · Cory House</i></p>

<p align="center"><b>¡Construyamos algo increíble juntos!</b> 🚀</p>
