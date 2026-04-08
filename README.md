<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  <img src="https://raw.githubusercontent.com/devloperdevesh/devloperdevesh/main/banner.png" width="100%" />
</p>
<p align="center">
  <a href="https://developerdevesh.vercel.app">
    <img src="https://img.shields.io/badge/Portfolio-000?style=for-the-badge&logo=vercel&logoColor=white"/>
  </a>
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
</p>

---

## ⚡ Engineering Activity
<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=devloperdevesh&show_icons=true" height="160"/>
  <img src="https://streak-stats.demolab.com?user=devloperdevesh&hide_border=true" height="160"/>
</p>

---

## 🧠 What I Build

- High-throughput distributed systems (validated under ~850 req/sec load)
- Async backend systems (non-blocking, high concurrency)
- RAG pipelines and vector search systems
- Multi-LLM orchestration and inference systems
- Distributed caching and latency optimization

---

## 🚀 Flagship System — Distributed AI Backend

Production-scale system designed for high-concurrency AI workloads.

### Scale
- ~850 req/sec throughput (validated under load)
- Designed for high-concurrency workloads
- 100K+ documents processed

### Architecture
- Async FastAPI microservices  
- Redis distributed caching  
- FAISS vector search  
- Kafka-based event pipelines  
- Multi-LLM routing layer  

### Engineering Decisions
- Stateless services for horizontal scaling  
- Async pipelines for non-blocking execution  
- Cache-first design to reduce inference cost  
- Backpressure handling for traffic stability  

### Impact
- ~40% latency reduction  
- ~30% cost reduction  
- Stable under sustained and burst traffic  

---

## 🧩 System Architecture

```mermaid
graph TD
    Client --> CDN
    CDN --> LB[Load Balancer]
    LB --> API[FastAPI Gateway]
    API --> Cache[Redis Cache]
    API --> Workers[Async Workers]
    Workers --> VectorDB[FAISS Index]
    VectorDB --> LLM[LLM Providers]
    LLM --> Response
