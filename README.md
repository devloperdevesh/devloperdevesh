<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Backend Engineer building distributed systems that stay reliable under real-world load
</p>

<p align="center">
  <b>850+ req/sec</b> · <b>sub-500ms latency</b> · async · Kafka · Redis
</p>

<p align="center">
  AI Infrastructure · High-Concurrency Systems · Low-Latency APIs
</p>

<p align="center">
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
</p>

---

## Engineering Activity

<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=devloperdevesh&show_icons=true" height="160"/>
  <img src="https://streak-stats.demolab.com?user=devloperdevesh&hide_border=true" height="160"/>
</p>

---
## Open Source

<p align="center">
  <img src="https://img.shields.io/badge/Open%20Source-Active-22c55e?style=for-the-badge&logo=github&logoColor=white"/>
</p>

<p align="center">
  <b>Distributed Systems • High-Concurrency APIs • AI Infrastructure</b>
</p>

<p align="center">
  <img 
    src="https://github-readme-activity-graph.vercel.app/graph?username=devloperdevesh&theme=github&hide_border=true"
    width="92%"
  />
</p>

<p align="center">
  <sub>Scaling real-world systems • Optimizing latency • Building in public 🚀</sub>
</p>

---

## What I Build

- High-concurrency backend systems (**500–850+ req/sec** under load)  
- Distributed AI systems (**RAG, LLM orchestration, vector search**)  
- Event-driven architectures (**Kafka, async pipelines**)  
- API-first platforms for integrations and automation  
- Low-latency systems optimized using caching, batching, and routing  

---

## Flagship System — High-Concurrency AI Platform

Production-grade distributed backend system designed to handle real-world AI workloads at scale.

### Scale

- **~850 req/sec** throughput (load-tested)  
- **500+ concurrent requests** with stable latency  
- **100K+ documents processed**  

### Architecture

- Async FastAPI services (stateless, horizontally scalable)  
- Redis distributed caching  
- FAISS vector index for semantic retrieval  
- Kafka-based event pipelines  
- Multi-LLM routing with fallback handling  

### Engineering Decisions

- Stateless architecture for horizontal scaling  
- Async pipelines for non-blocking execution  
- Cache-first design to reduce latency and cost  
- Backpressure handling for system stability  
- API-first approach for extensibility  

### Impact

- **~40% latency reduction**  
- **~30% cost reduction**  
- Stable under sustained and burst traffic  

---

## System Architecture

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
