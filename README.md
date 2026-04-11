<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Backend Engineer focused on high-concurrency distributed systems and AI infrastructure
</p>

<p align="center">
  Built systems handling <b>~850+ req/sec</b> with <b>sub-500ms latency</b> under load
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

## What I Build

- High-concurrency backend systems (**500–850+ req/sec**)  
- Distributed AI systems (**RAG, LLM orchestration, vector search**)  
- Event-driven architectures (**Kafka, async pipelines**)  
- API-first platforms for integrations and automation  
- Low-latency systems using caching, batching, and routing  

---

## Flagship System — High-Concurrency AI Platform

Production-grade distributed backend system designed to simulate real-world AI workloads at scale.

### Scale

- **~850 req/sec throughput** (load-tested)  
- **500+ concurrent requests with stable latency**  
- **100K+ documents processed**  

### Architecture

- Async **FastAPI services** (stateless, horizontally scalable)  
- **Redis caching layer** for latency optimization  
- **FAISS vector index** for semantic retrieval  
- **Kafka event pipelines** for decoupled processing  
- **Multi-LLM routing layer** with fallback handling  

### Engineering Decisions

- Stateless services for horizontal scalability  
- Async execution for non-blocking performance  
- Cache-first design to reduce latency and cost  
- Backpressure and queueing for traffic stability  
- API-first design for extensibility  

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
