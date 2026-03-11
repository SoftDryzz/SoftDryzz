<div align="center">

# Cristo Fernandez Tome

**Full-Stack Developer | Rust & TypeScript | Founder of [SoftDryzz](https://softdryzz.com)**

Construyo herramientas de seguridad, CLIs y aplicaciones de escritorio con foco en rendimiento y fiabilidad.

[![Website](https://img.shields.io/badge/softdryzz.com-111111?style=flat-square&logo=google-chrome&logoColor=white)](https://softdryzz.com)
[![Email](https://img.shields.io/badge/contact@softdryzz.com-111111?style=flat-square&logo=gmail&logoColor=white)](mailto:contact@softdryzz.com)

</div>

---

## Sobre mi

Soy desarrollador full-stack especializado en **Rust** y **TypeScript**. Mi trabajo se centra en herramientas de seguridad, aplicaciones de escritorio de alto rendimiento y utilidades CLI. Fundador de **SoftDryzz**, donde desarrollo software profesional y ofrezco servicios de consultoria digital.

Titulado en Desarrollo de Aplicaciones Multiplataforma (DAM), con certificaciones en Digitalizacion Empresarial (EOI) e Inteligencia Artificial (Founderz).

> *[Read in English](#english)*

---

## Actualmente trabajando en

- **Vaultic v2** — Nueva version del gestor de secretos con soporte para equipos, rotacion automatica de claves y plugins de integracion.
- **Cerberus Pro** — Version avanzada del monitor de seguridad con analisis de comportamiento, reglas personalizadas y reporting automatizado.

---

## Proyectos destacados

### [Vaultic v1.3 - Gestor de secretos CLI](https://github.com/SoftDryzz/vaultic)

*Herramienta CLI para gestionar secretos y configuracion de forma segura entre equipos, con sincronizacion basada en Git. Publicada en crates.io.*

`Rust`

- Cifrado robusto con age o GPG y soporte multi-recipient
- Sincronizacion via Git sin dependencias cloud
- Soporte multi-entorno (dev/staging/prod) con herencia inteligente
- Diff y comparacion de secretos entre archivos y entornos
- Deteccion automatica de variables ausentes o desincronizadas
- Registro de auditoria completo en formato JSON

---

### [Cerberus - Monitor de seguridad](https://github.com/SoftDryzz/Cerberus)

*Monitor de seguridad open-source para Windows con deteccion de amenazas en tiempo real.*

`Rust` `Tauri` `Svelte` `TypeScript` `SQLite`

- Monitor de procesos con puntuacion de riesgo (0-100)
- Analizador de ejecutables: hash, analisis PE, integracion VirusTotal
- Monitor de red con seguimiento de conexiones por proceso
- Diagnostico del sistema: programas de inicio y tareas programadas
- Alertas nativas con umbrales configurables
- 119 unit tests | Soporte bilingue (ES/EN)

---

### [ProjectManager v2.0 CLI](https://github.com/SoftDryzz/ProjectManager)

*Un comando para todos tus proyectos. Detecta el tipo y estandariza build/run/test con diagnosticos, seguridad y estadisticas.*

`Java` `Maven`

- Deteccion automatica de 12+ tipos de proyecto (Gradle, Maven, Node.js, .NET, Python, Rust, Go, Flutter, Docker...)
- Diagnosticos con `pm doctor`, escaneo de seguridad con `pm secure` y auditorias con `pm audit`
- Estadisticas de rendimiento: tiempos de build/test/run y tendencias
- 800+ tests | Multiplataforma (Windows, Linux, macOS)

---

### [Tower Rate Tier - Rate limiting por niveles para Tower](https://github.com/SoftDryzz/tower-rate-tier)

*Middleware de rate limiting por tiers para el ecosistema Tower. Permite definir limites por plan (free/pro/enterprise) con soporte para request cost, storage pluggable y headers estandar.*

`Rust` `Tower` `Tokio`

- Rate limiting por tier/plan configurable por el usuario
- Request cost: endpoints pesados consumen mas cuota
- Algoritmo GCRA para distribucion uniforme de carga
- Storage pluggable: in-memory o Redis
- Compatible con Axum, Actix, Hyper y cualquier servicio Tower

---

### [Overlord (Pandora) - Agente IA auto-evolutivo](https://github.com/SoftDryzz/project-pandora)

*Agente de IA local autonomo con auto-evolucion, consciencia de hardware, voz bilingue y autonomia progresiva. 9 fases de desarrollo completadas.*

`Python` `Rust` `Docker` `React` `FastAPI`

- Auto-evolucion real: optimiza sus propios prompts, herramientas y estrategias
- Consciencia de hardware: monitoriza GPU/CPU/RAM, detecta cuellos de botella y solicita mejoras
- Autonomia progresiva de 6 niveles con gateway de aprobacion humana y kill switch
- Voz bilingue (ES/EN) con Whisper, Kokoro y Silero VAD
- Ejecucion de codigo en sandbox Docker + web automation con Playwright
- Web UI (React/Vite) + CLI con dashboard en tiempo real (Rich)
- Modulos Rust de alto rendimiento via PyO3 | Memoria persistente con ChromaDB

---

## Stack tecnologico

**Lenguajes principales**

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3670A0?style=flat-square&logo=python&logoColor=ffdd54)
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)

**Frontend & Desktop**

![Svelte](https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white)
![React](https://img.shields.io/badge/React-20232a?style=flat-square&logo=react&logoColor=61DAFB)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

**Backend & Infra**

![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=flat-square&logo=node.js&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2671E5?style=flat-square&logo=githubactions&logoColor=white)

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=SoftDryzz&show_icons=true&theme=github_dark&include_all_commits=true&hide_border=true" height="165" />
  <img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=SoftDryzz&layout=compact&theme=github_dark&langs_count=8&hide_border=true" height="165" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=SoftDryzz&theme=github-compact&hide_border=true" />
</p>

---

## Contacto

| Email | Uso |
|---|---|
| **contact@softdryzz.com** | Consultas generales y colaboraciones |
| **security@softdryzz.com** | Vulnerabilidades y divulgacion responsable |
| **cristo@softdryzz.com** | Contacto directo |

[![Website](https://img.shields.io/badge/softdryzz.com-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://softdryzz.com)

---

<a id="english"></a>

## About me (English)

I'm a full-stack developer specializing in **Rust** and **TypeScript**. My work focuses on security tooling, high-performance desktop applications, and developer CLI utilities. I founded **SoftDryzz**, where I build professional software and provide digital consulting services.

**Currently working on:** Vaultic v2 (secrets manager with team support) and Cerberus Pro (advanced security monitor with behavioral analysis).

**Featured projects:** [Vaultic](https://github.com/SoftDryzz/vaultic) — secrets manager CLI in Rust | [Cerberus](https://github.com/SoftDryzz/Cerberus) — Windows security monitor | [ProjectManager](https://github.com/SoftDryzz/ProjectManager) — unified project CLI | [Tower Rate Tier](https://github.com/SoftDryzz/tower-rate-tier) — tier-based rate limiting for Tower | [Project Pandora](https://github.com/SoftDryzz/project-pandora) — autonomous local AI agent.

---

<p align="center">
  <a href="https://github.com/sponsors/SoftDryzz">
    <img src="https://img.shields.io/badge/Sponsor-ea4aaa?style=flat-square&logo=github-sponsors&logoColor=white" alt="GitHub Sponsors">
  </a>
  &nbsp;
  <a href="https://buymeacoffee.com/xtoftomeo">
    <img src="https://img.shields.io/badge/Buy_me_a_coffee-FFDD00?style=flat-square&logo=buy-me-a-coffee&logoColor=black" alt="Buy Me A Coffee">
  </a>
  &nbsp;
  <img src="https://komarev.com/ghpvc/?username=softdryzz&style=flat-square&color=555555" alt="Profile views"/>
</p>
