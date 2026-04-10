<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Backend Engineer building scalable distributed systems and AI infrastructure
</p>

<p align="center">
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/devloperdevesh/devloperdevesh/main/banner.png" width="80%" />
</p>

---

## Engineering Activity

<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=devloperdevesh&show_icons=true" height="160"/>
  <img src="https://streak-stats.demolab.com?user=devloperdevesh&hide_border=true" height="160"/>
</p>

---

## What I Build

- High-concurrency backend systems handling **500–850+ req/sec under load**  
- Distributed AI systems (**RAG, LLM orchestration, vector search**)  
- API-first systems designed for **external integrations and automation workflows**  
- Event-driven architectures using **Kafka and async pipelines**  
- Low-latency systems optimized using **caching, batching, and routing strategies**  

---

## Flagship System — High-Concurrency AI API Platform

Production-grade distributed backend system designed for scalable AI workloads and real-world traffic.

### Scale
- **~850 req/sec throughput** (load-tested)  
- **500+ concurrent requests handled with stable latency**  
- **100K+ documents processed**  

### Architecture
- Async **FastAPI microservices** (stateless, horizontally scalable)  
- **Redis distributed caching** for low-latency performance  
- **FAISS vector search** for efficient semantic retrieval  
- **Kafka-based event pipelines** for async and decoupled processing  
- **Multi-LLM routing layer** with intelligent fallback handling  

### Engineering Decisions
- Stateless services enabling horizontal scaling  
- Async pipelines for non-blocking execution  
- Cache-first design to reduce latency and inference cost  
- Queueing and backpressure handling for traffic stability  
- API-first design enabling integration into external systems  

### Impact
- **~40% latency reduction**  
- **~30% cost reduction**  
- Stable under sustained and burst traffic conditions  

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
