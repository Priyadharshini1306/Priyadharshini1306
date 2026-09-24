<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:2C5364,100:36BCF7&height=230&section=header&text=Priyadharshini%20R&fontSize=58&fontColor=ffffff&fontAlignY=38&desc=Java%20Full%20Stack%20Developer%20%7C%20AI%20%26%20Data%20Science&descSize=20&descAlignY=60&animation=fadeIn" width="100%" alt="header" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=36BCF7&center=true&vCenter=true&width=850&height=60&lines=I+build+production-style+full-stack+applications;Java+%7C+Spring+Boot+%7C+React+%7C+REST+APIs;Now+building+RAG+%2B+Knowledge+Graphs+%2B+GenAI;Code+%E2%80%A2+Build+%E2%80%A2+Deploy+%E2%80%A2+Improve" alt="typing" />

<br/>

**B.E. Artificial Intelligence & Data Science** · Bannari Amman Institute of Technology

<br/>

<a href="https://www.linkedin.com/in/priyadharshini-r-dev/"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
<a href="https://github.com/Priyadharshini1306"><img src="https://img.shields.io/badge/-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>&nbsp;
<a href="https://leetcode.com/u/Priyadharshini1306/"><img src="https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>&nbsp;
<a href="mailto:priyarajan1306@gmail.com"><img src="https://img.shields.io/badge/-Email%20Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

<br/><br/>

<a href="https://car-booking-app-2-46gs.onrender.com/"><img src="https://img.shields.io/badge/-%F0%9F%9A%80%20View%20Live%20Project-00C853?style=for-the-badge" alt="Live Project" /></a>&nbsp;
<img src="https://img.shields.io/badge/-%F0%9F%9F%A2%20Open%20to%20Internships%20%26%20Full%20Time%20Roles-1F2937?style=for-the-badge" alt="Open to work" />

</div>

---

## 👩‍💻 About Me

I'm a **Java Full Stack Developer** and **AI & Data Science** undergraduate who enjoys turning ideas into **complete, working, deployed products**, not just tutorial code.

I think in layers and own the whole pipeline:

```text
Backend  ➜  REST APIs  ➜  Database  ➜  Frontend  ➜  Deployment
```

**What sets me apart:** I combine solid **backend engineering** (secure APIs, role-based access, data integrity) with hands-on **applied AI** (RAG pipelines, knowledge graphs, LLM workflows).

### 🎯 Currently Focused On

| Area | What I'm doing |
|------|----------------|
| ☕ **Java & Spring Boot** | Building secure, scalable REST backends |
| ⚛️ **React.js** | Component-driven, responsive UIs |
| 🧩 **DSA** | Regular problem solving on LeetCode |
| 🤖 **Generative AI** | RAG, LangChain, LangGraph, local LLMs |
| ☁️ **Cloud & 🐳 DevOps** | Docker, cloud deployment, CI/CD basics |

---

## ⚡ Tech Stack

<div align="center">

| | |
|---|---|
| **Languages** | ![Languages](https://skillicons.dev/icons?i=java,python,c,cpp,js&theme=dark) |
| **Frontend** | ![Frontend](https://skillicons.dev/icons?i=html,css,react,tailwind&theme=dark) |
| **Backend** | ![Backend](https://skillicons.dev/icons?i=spring,fastapi,python&theme=dark) |
| **Databases** | ![Databases](https://skillicons.dev/icons?i=mysql,mongodb,neo4j&theme=dark) |
| **Tools & DevOps** | ![Tools](https://skillicons.dev/icons?i=git,github,docker,postman,vscode,idea&theme=dark) |

</div>

**AI / GenAI stack:** `LangChain` · `LangGraph` · `RAG` · `Qdrant (Vector DB)` · `Neo4j (Knowledge Graph)` · `Ollama (Local LLMs)`

---

## 🚀 Featured Projects

### 🚗 01 · Car Booking Application
**Full-stack vehicle booking & fleet management platform**

<a href="https://car-booking-app-2-46gs.onrender.com/"><img src="https://img.shields.io/badge/-%F0%9F%9A%80%20Live%20Demo-00C853?style=for-the-badge" alt="Live Demo" /></a>&nbsp;
<a href="https://github.com/Priyadharshini1306/car-booking-app"><img src="https://img.shields.io/badge/-Source%20Code-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source Code" /></a>

`Java` `Spring Boot` `Spring Security` `MySQL` `WebSockets` `HTML` `CSS` `JavaScript` `Render`

A complete platform that manages **vehicles, bookings, drivers, users and administrators**, with real-time communication and automated compliance tracking.

<table>
<tr>
<td width="50%" valign="top">

**🔐 Security & Access**
- Authentication & authorization
- USER / ADMIN role-based access
- Secure REST APIs with Spring Security

**🚘 Booking Engine**
- Advanced vehicle search & filtering
- Hourly and daily booking
- Booking **overlap prevention**
- Driver assignment
- Ratings & feedback system

</td>
<td width="50%" valign="top">

**🛠️ Operations & Admin**
- Vehicle maintenance management
- Driver shift & leave management
- Vehicle document expiry monitoring
- Driver license expiry monitoring

**🔔 Real-Time**
- Live user ↔ admin communication via WebSockets

</td>
</tr>
</table>

**🧱 Architecture**

```mermaid
flowchart LR
    A[Web Client<br/>HTML · CSS · JS] -->|REST| B[Spring Boot API]
    A <-->|WebSocket| B
    B --> C[Spring Security<br/>USER / ADMIN]
    B --> D[(MySQL)]
    B --> E[Booking Engine<br/>Overlap Prevention]
    B --> F[Expiry Monitoring<br/>Documents & Licenses]
```

**💡 Engineering highlights**
- Designed booking logic that prevents **double-booking** for the same vehicle and time window
- Separated concerns across controller, service and repository layers
- Deployed end-to-end on **Render** as a live, publicly usable application

---

### 🧠 02 · CurriculumMind AI
**AI-powered curriculum analysis & personalized learning platform**

<img src="https://img.shields.io/badge/-%F0%9F%9A%A7%20In%20Development-F97316?style=for-the-badge" alt="In Development" />

`Python` `FastAPI` `React.js` `LangChain` `LangGraph` `RAG` `Neo4j` `Qdrant` `MongoDB` `Ollama`

An AI system I'm currently building that reads academic syllabus documents and converts them into a **structured knowledge graph**, finds matching learning resources, detects **knowledge gaps**, and generates **quizzes and personalized learning paths**.

**🔥 Core Workflow**

```mermaid
flowchart TD
    A[📄 Syllabus Upload] --> B[Text Extraction]
    B --> C[🤖 AI Curriculum Analysis]
    C --> D[Course / Unit / Topic Extraction]
    D --> E{👤 Human Review<br/>& Correction}
    E --> F[🕸️ Knowledge Graph<br/>Neo4j]
    F --> G[Resource Discovery]
    G --> H[Semantic Matching<br/>Qdrant Vector Search]
    H --> I[Coverage Analysis]
    I --> J[Knowledge Gap Detection]
    J --> K[📝 Quiz Generation]
    K --> L[🎯 Personalized Learning Path]
```

**💡 Design highlights**
- **Human-in-the-loop** review step so AI output is corrected before it enters the knowledge graph
- **Hybrid retrieval:** graph relationships (Neo4j) combined with semantic similarity (Qdrant)
- Runs on **local LLMs via Ollama**, so there is no dependency on paid APIs
- Agent-style pipeline orchestrated with **LangGraph**

---

## 📊 GitHub Stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Priyadharshini1306&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Priyadharshini1306&layout=compact&theme=tokyonight&hide_border=true" alt="languages" />

<img src="https://streak-stats.demolab.com?user=Priyadharshini1306&theme=tokyonight&hide_border=true" alt="streak" />

</div>

---

## 🗺️ Roadmap

- [x] Full-stack Java application with security, real-time features and cloud deployment
- [ ] 🚧 CurriculumMind AI: RAG pipeline, knowledge graph and personalized learning paths (in progress)
- [ ] Dockerize and add CI/CD pipelines to all projects
- [ ] Deploy Spring Boot + React architecture on cloud
- [ ] Keep growing on LeetCode (DSA consistency)
- [ ] Contribute to open-source

---

## 🤝 Let's Connect

I'm looking for **internship and entry-level opportunities** in **Java / Full Stack / AI-enabled development**.

<div align="center">

<a href="https://www.linkedin.com/in/priyadharshini-r-dev/"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
<a href="mailto:priyarajan1306@gmail.com"><img src="https://img.shields.io/badge/-priyarajan1306@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>&nbsp;
<a href="https://leetcode.com/u/Priyadharshini1306/"><img src="https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>

<br/><br/>

*"Make it work, make it right, make it fast."*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:36BCF7,50:2C5364,100:0F2027&height=120&section=footer" width="100%" alt="footer" />

</div>
