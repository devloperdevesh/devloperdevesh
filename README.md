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
  <img src="https://github-readme-stats.vercel.app/api?username=devloperdevesh&show_icons=true&hide_border=true" height="160"/>
  <img src="https://streak-stats.demolab.com/?user=devloperdevesh&hide_border=true" height="160"/>
</p>

---

## What I Build

- High-throughput RAG systems (100K+ documents)
- Async backend systems (1K+ concurrency)
- Multi-LLM orchestration backends
- Distributed caching and low-latency inference systems

---

## Flagship System — Distributed AI Backend

Production-grade backend system designed for high-concurrency AI workloads.

**Scale**
- 100K+ documents processed  
- 1K+ concurrent requests  

**Architecture**
- Async FastAPI services  
- Redis distributed caching  
- FAISS vector search  
- Multi-LLM routing layer  

**Engineering Decisions**
- Stateless services for horizontal scaling  
- Non-blocking async pipelines for throughput  
- Cache-first design to reduce inference load  
- Optimized vector indexing for fast retrieval  

**Impact**
- p95 latency reduced by 40%  
- Inference cost reduced by 30%  
- Stable under sustained concurrent load  

---

## Open Source Contributions

- Contributing to OpenVINO (FastAPI-based inference systems)
- Extended inference examples with async handling, batching, and logging

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


