<h1 align="center">Devesh Chauhan</h1>

<p align="center">
AI Backend Engineer — Distributed Systems & LLM Infrastructure
</p>

<p align="center">
Building systems handling <strong>1K+ concurrent users</strong> and <strong>100K+ documents</strong> with optimized latency and cost
</p>

<p align="center">
<strong>Latency ↓ 40%</strong> • <strong>Cost ↓ 30%</strong>
</p>

<p align="center">
  <a href="https://developerdevesh.vercel.app">
    <img src="https://img.shields.io/badge/Portfolio-000?style=for-the-badge&logo=vercel&logoColor=white"/>
  </a>
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://leetcode.com/u/devloperdevesh">
    <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black"/>
  </a>
</p>

---

## Engineering Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=devloperdevesh&show_icons=true&theme=github_dark&hide_border=true" height="150"/>
  <img src="https://streak-stats.demolab.com/?user=devloperdevesh&theme=github-dark-blue&hide_border=true" height="150"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=devloperdevesh&layout=compact&theme=github_dark&hide_border=true" height="150"/>
</p>

---

## What I Build

- High-throughput RAG systems (100K+ documents)
- Async backend systems (1K+ concurrency)
- Multi-LLM orchestration backends
- Distributed caching and low-latency inference systems

---

## Flagship System — Distributed AI Backend

Production-grade AI backend designed for real-world scale.

**Scale**
- 100K+ documents
- 1K+ concurrent users

**Architecture**
- FastAPI (async services)
- Redis (distributed caching)
- FAISS (vector search)
- Multi-LLM routing

**Key Decisions**
- Stateless services for horizontal scaling  
- Async request handling to remove blocking  
- Caching layer to reduce repeated inference  
- Vector index optimization for faster retrieval  

**Impact**
- Reduced latency by 40% (p95)  
- Reduced inference cost by 30%  
- Stable performance under high concurrency  

---

## System Architecture

```mermaid
graph TD
    User --> API[FastAPI Gateway]
    API --> Cache[Redis Cache]
    API --> Workers[Async Workers]
    Workers --> VectorDB[FAISS Index]
    VectorDB --> LLM[LLM Providers]
    LLM --> Response
