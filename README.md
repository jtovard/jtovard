<!-- Paleta neon BuzumAIcenter: #0d0021 #120033 #f72585 #4cc9f0 #b5179e #7bf1a8 #f9c74f #ff4d6d -->
<div align="center">
  <img src="assets/header-neon.svg" alt="Jota — BuzumAIcenter synthwave header" width="92%" />
</div>

<div align="center">

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white&labelColor=0d0021)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white&labelColor=120033)](https://fastapi.tiangolo.com/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white&labelColor=1a0040)](https://www.docker.com/)
[![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black&labelColor=0d0021)](https://www.linux.org/)

[![Agents](https://img.shields.io/badge/CrewAI_agents-f72585?style=for-the-badge&labelColor=120033)](https://github.com/jtovard/buzumAIcenter)
[![LLM](https://img.shields.io/badge/Ollama_%7C_RAG-4cc9f0?style=for-the-badge&labelColor=0d0021)](https://github.com/jtovard/buzumAIcenter)
[![SQLite](https://img.shields.io/badge/SQLite_WAL-b5179e?style=for-the-badge&logo=sqlite&logoColor=white&labelColor=120033)](https://www.sqlite.org/)

[![Laravel](https://img.shields.io/badge/Laravel-ff4d6d?style=for-the-badge&logo=laravel&logoColor=white&labelColor=120033)](https://laravel.com/)
[![Cursor](https://img.shields.io/badge/Cursor_%7C_Claude-f9c74f?style=for-the-badge&labelColor=1a0040)](https://cursor.com/)
[![MCP](https://img.shields.io/badge/MCP_integrations-7bf1a8?style=for-the-badge&labelColor=0d0021)](https://modelcontextprotocol.io/)
[![Hermes](https://img.shields.io/badge/Hermes_Agent-f72585?style=for-the-badge&labelColor=120033)](https://github.com/NousResearch/hermes-agent)
[![Anthropic](https://img.shields.io/badge/Anthropic_Claude-d97757?style=for-the-badge&labelColor=1a0040)](https://www.anthropic.com/)
[![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white&labelColor=120033)](https://playwright.dev/)

</div>

<br/>

<div align="center">

### ⚡ En foco ahora

</div>

<table align="center">
<tr><td align="center" width="33%">

[![BuzumAIcenter](https://img.shields.io/badge/repo-BuzumAIcenter-f72585?style=for-the-badge&logo=github&logoColor=white&labelColor=120033)](https://github.com/jtovard/buzumAIcenter)

<strong>Servidor AI dockerizado</strong> · FastAPI · CrewAI · Ollama · ChromaDB · Obsidian RAG · Telegram · MCP/Cursor<br/><br/>
🎯 Señales <strong>watchlist ∪ cartera</strong> · digest <strong>noticias ×5</strong> · <strong>capa conversacional</strong> (LLM + MCP custom)

</td><td align="center" width="33%">

[![Pi gateway](https://img.shields.io/badge/hardware-Raspberry_Pi-7bf1a8?style=for-the-badge&logo=raspberrypi&logoColor=black&labelColor=0d0021)](https://github.com/jtovard/buzumAIcenter)

<strong>Siempre encendido</strong>: news API/collector/scorer, Chroma, vault watcher, bot · LLM por proxy a la PC

</td><td align="center" width="33%">

[![COR](https://img.shields.io/badge/product-COR-f9c74f?style=for-the-badge&labelColor=1a0040&logoColor=000)](https://projectcor.com/)

<strong>Engineering Manager</strong> · roadmap técnico · habilitar al equipo con IA<br/><br/>
🏗 <strong>Plataforma agéntica</strong>: hub <code>cor-agents</code> + agentes por dominio (bugs, migraciones Support)<br/>
📋 <strong>SDLC</strong> en Cursor · skills Claude · MCP COR · Laravel/PHP · E2E Playwright

</td></tr>
</table>

<br/>

<div align="center">

### 🧠 Dominios

</div>

| | |
|:---:|:---|
| ![](https://img.shields.io/badge/-Backend_%26_datos-4cc9f0?style=flat-square&labelColor=120033) | Python, FastAPI, SQLite (WAL), PHP/Symfony/Laravel, Node.js, PostgreSQL, MySQL |
| ![](https://img.shields.io/badge/-AI_%26_automatización-f72585?style=flat-square&labelColor=120033) | Multi-agente, prompts operativos, RAG, embeddings locales, integración MCP |
| ![](https://img.shields.io/badge/-Agentes_conversacionales-4cc9f0?style=flat-square&labelColor=120033) | Diseño de asistentes always-on con memoria persistente · MCP servers custom · guardrails anti-alucinación · tool use sobre Anthropic / Claude |
| ![](https://img.shields.io/badge/-Mercados_(personal)-b5179e?style=flat-square&labelColor=120033) | Indicadores, alertas Telegram, guardrails — **DYOR**, no es asesoramiento financiero |
| ![](https://img.shields.io/badge/-Infra-7bf1a8?style=flat-square&labelColor=0d0021) | Docker, Linux, despliegues hogar/LAN, GitHub Actions, workspace monorepo |
| ![](https://img.shields.io/badge/-Engineering_leadership-f9c74f?style=flat-square&labelColor=1a0040) | Roadmap técnico, priorización, deuda, alineamiento con producto/stakeholders, estándares de equipo |
| ![](https://img.shields.io/badge/-Plataforma_agéntica_(COR)-ff4d6d?style=flat-square&labelColor=120033) | Ver tabla abajo — flujos operativos versionados, no prompts sueltos |

<br/>

<div align="center">

### 🏗 COR · Patrones & arquitectura (highlights recientes)

</div>

<table align="center">
<tr><td width="50%" valign="top">

**Arquitectura hub-and-spoke**

- Hub `cor-agents`: registry YAML, `agent.manifest.yaml`, `link-agents.py`
- Un repo por agente (`bug-resolver`, `support-migrations`) — sin duplicar KB
- Workspace `cor/` · rules Cursor · skills Claude · mensajes stakeholder vía proxy *Agente Smith*

**Proceso agnóstico de herramienta**

- `core/` (contratos, playbooks) + `adapters/` (Cursor, Claude)
- Verificable por AI: `link-agents.py --verify --json`

</td><td width="50%" valign="top">

**Agentes en producción (privados)**

| Agente | Qué estandariza |
|--------|-----------------|
| **bug-resolver** | Triage → dossier → repro local → fix acotado → PR legible `(COR-id)` |
| **support-migrations** | Tickets Support → migraciones Laravel parametrizables + KB de templates |

**Stack & disciplina**

- PHP/Laravel, migraciones multi-tenant, guardias de ambiente
- Playwright + PHPUnit · branches desde tag deployado · PRs quirúrgicos
- Integración ticket COR (MCP): claim, updates HTML para PM/QA

</td></tr>
</table>

<br/>

<div align="center">

### 🧭 Enfoque EM · roadmap

</div>

| | |
|:---:|:---|
| **Priorizar** | Impacto en cliente, riesgo, deuda que bloquea velocidad — no “nice to have” infinito |
| **Estandarizar** | Playbooks y agentes para que el equipo repita calidad sin depender de una persona |
| **Medir** | Bugs con trazabilidad, migraciones con templates, PRs revisables en minutos |
| **Comunicar** | Lenguaje claro hacia producto/QA (updates COR, no jerga de diff interno) |

<br/>

<div align="center">

### 📫 Contacto & redes

**josemigueltovarduarte@gmail.com** · [LinkedIn](https://www.linkedin.com/in/josemitovard/)

<br/>

[![Dev.to](https://img.shields.io/badge/dev.to-buzusuma-0A0A0A?style=for-the-badge&logo=devdotto&logoColor=white&labelColor=3d0080)](https://dev.to/buzusuma)
[![Twitter](https://img.shields.io/badge/Twitter-jmi_t-4cc9f0?style=for-the-badge&logo=x&logoColor=white&labelColor=120033)](https://twitter.com/jmi_t)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jota-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=1a0040)](https://www.linkedin.com/in/josemitovard/)
[![Instagram](https://img.shields.io/badge/Instagram-josemitovar-E4405F?style=for-the-badge&logo=instagram&logoColor=white&labelColor=120033)](https://instagram.com/josemitovar)

<br/>

### 🛠 Stack (neon badges)

[![Py](https://img.shields.io/badge/Python-f72585?style=flat-square&logo=python&logoColor=white&labelColor=120033)](https://www.python.org/)
[![Fa](https://img.shields.io/badge/FastAPI-4cc9f0?style=flat-square&logo=fastapi&logoColor=0d0021&labelColor=e0d7ff)](https://fastapi.tiangolo.com/)
[![Dock](https://img.shields.io/badge/Docker-b5179e?style=flat-square&logo=docker&logoColor=white&labelColor=120033)](https://www.docker.com/)
[![Lin](https://img.shields.io/badge/Linux-f9c74f?style=flat-square&logo=linux&logoColor=black&labelColor=1a0040)](https://www.linux.org/)
[![Git](https://img.shields.io/badge/Git-ff4d6d?style=flat-square&logo=git&logoColor=white&labelColor=120033)](https://git-scm.com/)
[![JS](https://img.shields.io/badge/JavaScript-7bf1a8?style=flat-square&logo=javascript&logoColor=black&labelColor=0d0021)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![TS](https://img.shields.io/badge/TypeScript-4cc9f0?style=flat-square&logo=typescript&logoColor=white&labelColor=120033)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-f72585?style=flat-square&logo=react&logoColor=white&labelColor=120033)](https://reactjs.org/)
[![Next](https://img.shields.io/badge/Next.js-e0d7ff?style=flat-square&logo=nextdotjs&logoColor=black&labelColor=1a0040)](https://nextjs.org/)
[![Node](https://img.shields.io/badge/Node-7bf1a8?style=flat-square&logo=nodedotjs&logoColor=black&labelColor=0d0021)](https://nodejs.org/)
[![PHP](https://img.shields.io/badge/PHP-9b87c4?style=flat-square&logo=php&logoColor=white&labelColor=120033)](https://www.php.net/)
[![Sym](https://img.shields.io/badge/Symfony-000000?style=flat-square&logo=symfony&logoColor=white&labelColor=3d0080)](https://symfony.com/)
[![Lar](https://img.shields.io/badge/Laravel-ff4d6d?style=flat-square&logo=laravel&logoColor=white&labelColor=120033)](https://laravel.com/)
[![Pg](https://img.shields.io/badge/PostgreSQL-4cc9f0?style=flat-square&logo=postgresql&logoColor=white&labelColor=120033)](https://www.postgresql.org/)
[![My](https://img.shields.io/badge/MySQL-f9c74f?style=flat-square&logo=mysql&logoColor=black&labelColor=1a0040)](https://www.mysql.com/)
[![Redis](https://img.shields.io/badge/Redis-f72585?style=flat-square&logo=redis&logoColor=white&labelColor=120033)](https://redis.io/)
[![Pandas](https://img.shields.io/badge/Pandas-130754?style=flat-square&logo=pandas&logoColor=white&labelColor=120033)](https://pandas.pydata.org/)
[![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white&labelColor=120033)](https://aws.amazon.com/)
[![GQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white&labelColor=1a0040)](https://graphql.org/)
[![Cursor](https://img.shields.io/badge/Cursor-f9c74f?style=flat-square&labelColor=1a0040)](https://cursor.com/)
[![PW](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white&labelColor=120033)](https://playwright.dev/)
[![YAML](https://img.shields.io/badge/YAML_manifests-4cc9f0?style=flat-square&labelColor=120033)](https://yaml.org/)
[![GHA](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white&labelColor=0d0021)](https://github.com/features/actions)

<details>
<summary><b>Más herramientas (legacy)</b></summary>

[![Babel](https://img.shields.io/badge/Babel-F9DC3E?style=flat-square&logo=babel&logoColor=black&labelColor=120033)](https://babeljs.io/)
[![Chart](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white&labelColor=120033)](https://www.chartjs.org/)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white&labelColor=0d0021)](https://www.w3schools.com/css/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white&labelColor=120033)](https://www.w3.org/html/)
[![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white&labelColor=1a0040)](https://www.jenkins.io/)
[![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white&labelColor=120033)](https://postman.com/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white&labelColor=120033)](https://pytorch.org/)
[![SK](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white&labelColor=1a0040)](https://scikit-learn.org/)
[![TF](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white&labelColor=120033)](https://www.tensorflow.org/)
[![Webpack](https://img.shields.io/badge/Webpack-8DD6F9?style=flat-square&logo=webpack&logoColor=black&labelColor=0d0021)](https://webpack.js.org/)
[![Zapier](https://img.shields.io/badge/Zapier-FF4F00?style=flat-square&logo=zapier&logoColor=white&labelColor=120033)](https://zapier.com/)

</details>

</div>

---

<div align="center">

⚡ **Extra:** piano · videojuegos · entrenar · tiempo con amigos

[![trophy](https://github-profile-trophy.vercel.app/?username=jtovard&theme=dracula&column=7&margin-w=10&margin-h=10)](https://github.com/ryo-ma/github-profile-trophy)

<img src="https://github-readme-streak-stats.herokuapp.com/?user=jtovard&theme=tokyonight&ring=f72585&fire=f72585&currStreakLabel=4cc9f0" alt="GitHub streak" />

</div>
