<div align="center">

# Hi, I'm Priyadharshini R 👋

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=36BCF7&center=true&vCenter=true&width=850&height=60&lines=Full-Stack+Developer+%7C+Applied+AI+Engineer;Java+%7C+Spring+Boot+%7C+Python+%7C+FastAPI+%7C+React;Knowledge+Graphs+%2B+LLM+Pipelines+%2B+Vector+Search;I+ship+tested%2C+secure%2C+deployed+software" alt="typing" />

**B.E. Artificial Intelligence & Data Science** · Bannari Amman Institute of Technology
**Oracle Certified Professional: Java SE 17 Developer**

<a href="https://www.linkedin.com/in/priyadharshini-r-dev/"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
<a href="mailto:priyarajan1306@gmail.com"><img src="https://img.shields.io/badge/-Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>&nbsp;
<a href="https://leetcode.com/u/Priyadharshini1306/"><img src="https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>&nbsp;
<img src="https://img.shields.io/badge/-Open%20to%20Internships%20%26%20Full--Time%20Roles-00C853?style=for-the-badge" alt="Open to work" />

</div>

---

## 🚀 About Me

I build **complete, production-style applications** — from secure backends and database design to polished UIs and AI pipelines — and I test and deploy what I build.

```text
Problem ➜ Architecture ➜ Backend & APIs ➜ Databases ➜ AI Pipeline ➜ Frontend ➜ Tests ➜ Deploy
```

- 🧩 **Backend engineering:** secure REST APIs, JWT & role-based access, data integrity, clean layered architecture
- 🤖 **Applied AI:** LLM pipelines with validated structured output, knowledge graphs, vector search, adaptive systems
- ✅ **Engineering discipline:** unit, integration and end-to-end tests; documented limitations; no secrets in code

---

## ⭐ Featured Projects

### 01 · CurriculumMind AI — Syllabus ➜ Knowledge Graph ➜ Adaptive Study Plan

<img src="https://img.shields.io/badge/Status-Working%20End--to--End-00C853?style=for-the-badge" alt="Status" />&nbsp;
<a href="https://github.com/Priyadharshini1306/curriculummind-ai"><img src="https://img.shields.io/badge/-Source%20Code-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source Code" /></a>

`Python` `FastAPI` `React` `Neo4j` `MongoDB` `Groq LLM` `sentence-transformers` `Docling` `NetworkX` `Cytoscape.js` `Tailwind`

Upload a syllabus (PDF, DOCX, PPTX, text or a **scanned image**) or simply describe a learning goal. CurriculumMind builds a **concept knowledge graph with prerequisites**, schedules it into a **week-by-week semester plan**, discovers and ranks **learning resources** for every concept, **quizzes** the learner, and **re-plans the path** around their weak spots.

```mermaid
flowchart LR
    A["Syllabus / Goal"] --> B["Docling + OCR"]
    B --> C["LLM Extraction"]
    C --> V1{"Human Review 1"}
    V1 --> D["Concepts & Prerequisites"]
    D --> G["Graph Validation"]
    G --> V2{"Human Review 2"}
    V2 --> N[("Neo4j Graph")]
    N --> S["Topological Sort + Week Allocation"]
    S --> V3{"Human Review 3"}
    V3 --> R["Resource Discovery + Vector Matching"]
    R --> CV["Coverage & Gap Loop"]
    CV --> Q["Quizzes"]
    Q --> M["Mastery"]
    M --> AP["Adaptive Path"]
    AP --> Q
```

**What makes it engineering-grade**

| | |
|---|---|
| 🛡️ **LLM output is never trusted** | Structured JSON ➜ Pydantic validation (retry with error fed back) ➜ business rules (duplicates, unknown names, cycles, invalid questions dropped) ➜ human review ➜ database |
| 🧠 **Graph algorithms** | Cycle / DAG checks, transitive-edge reduction and orphan detection (NetworkX); topological sort + workload-constrained semester & week allocation |
| 🔎 **Semantic resource matching** | 384-d embeddings stored in **Neo4j vector indexes**; evidence-based coverage %, duplicate detection, heuristic version checks |
| 🔁 **Bounded gap loop** | Targeted re-search for uncovered concepts, capped at 3 iterations, then flagged `UNRESOLVED_GAP` for the instructor |
| 📈 **Adaptive learning loop** | Quiz ➜ per-concept mastery ➜ root-cause prerequisite gaps ➜ reshuffled path ➜ quiz again |
| 🗄️ **Polyglot persistence** | MongoDB Atlas for users, sessions, drafts and quiz history · Neo4j AuraDB for the knowledge graph, linked only by `user_id` |
| 🔐 **Security** | bcrypt, JWTs bound to server-side sessions (real logout), login throttling, upload signature checks, owner-scoped data, instructor-only endpoints, answers never sent before submission |
| ✅ **Tested** | **90 offline unit tests** + integration tests against live services + full-pipeline **E2E tests** through the HTTP API |

**By the numbers:** 3 human-in-the-loop gates · 2 databases · 40+ REST endpoints across 12 modules · 5 input formats incl. OCR · learner & instructor dashboards

---

### 02 · Car Booking Application — Vehicle Booking & Fleet Management

<a href="https://car-booking-app-2-46gs.onrender.com/"><img src="https://img.shields.io/badge/-Live%20Demo-00C853?style=for-the-badge" alt="Live Demo" /></a>&nbsp;
<a href="https://github.com/Priyadharshini1306/car-booking-app"><img src="https://img.shields.io/badge/-Source%20Code-181717?style=for-the-badge&logo=github&logoColor=white" alt="Source Code" /></a>

`Java` `Spring Boot` `Spring Security` `MySQL` `WebSockets` `JavaScript` `Render`

A deployed platform managing **vehicles, bookings, drivers, users and admins**, with real-time messaging and automated compliance tracking.

- 🔐 **USER / ADMIN role-based access** with Spring Security
- 📅 **Booking engine** with hourly/daily booking and **double-booking prevention** for the same vehicle and time window
- 🧑‍✈️ Driver assignment, shifts, leave, ratings and feedback
- ⏰ **Expiry monitoring** for vehicle documents and driver licenses
- ⚡ **Live user ↔ admin chat** over WebSockets
- 🏗️ Layered controller ➜ service ➜ repository design, deployed end-to-end on Render

```mermaid
flowchart LR
    A["Web Client"] -->|REST| B["Spring Boot API"]
    A <-->|WebSocket| B
    B --> C["Spring Security"]
    B --> E["Booking Engine"]
    B --> F["Expiry Monitoring"]
    B --> D[("MySQL")]
```

---

## 🛠️ Tech Stack

| | |
|---|---|
| **Languages** | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black) |
| **Backend** | ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white) |
| **Frontend** | ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) |
| **Databases** | ![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?style=flat-square&logo=neo4j&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| **AI / ML** | ![LLM APIs](https://img.shields.io/badge/Groq%20%7C%20Ollama-111827?style=flat-square) ![Embeddings](https://img.shields.io/badge/sentence--transformers-FF6F00?style=flat-square) ![RAG](https://img.shields.io/badge/RAG-7C3AED?style=flat-square) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![Knowledge Graphs](https://img.shields.io/badge/Knowledge%20Graphs-008CC1?style=flat-square) |
| **Testing & DevOps** | ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) ![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black) |

---

## 🏆 Certifications

<div align="center">

<img width="402" height="298" alt="Oracle Certified Professional Java SE 17 Developer" src="https://github.com/user-attachments/assets/8b6c8411-08c8-4058-9d42-7628ae2aa4b9" />

**Oracle Certified Professional**

</div>

---

## 🗺️ What's Next

- [x] Deployed full-stack Java app with security and real-time features
- [x] CurriculumMind AI: knowledge graph, semester sequencing, resource coverage and adaptive learning loop
- [ ] CurriculumMind AI: Celery + Redis workers, Docker, CI/CD and cloud deployment
- [ ] Spring Boot + React application deployed on cloud
- [ ] Consistent DSA practice on LeetCode · open-source contributions

---

<div align="center">

### 🤝 Let's Connect

Looking for **internship and entry-level roles** in **Java / Full-Stack / AI-enabled development**.

<a href="https://www.linkedin.com/in/priyadharshini-r-dev/"><img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>&nbsp;
<a href="mailto:priyarajan1306@gmail.com"><img src="https://img.shields.io/badge/-priyarajan1306@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

*"Make it work, make it right, make it fast."*

</div>
