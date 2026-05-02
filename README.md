<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Backend Engineer building distributed systems that stay reliable under real-world load
</p>

<p align="center">
  850+ req/sec · sub-500ms latency · async · Kafka · Redis
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

## What I Build

- High-concurrency backend systems (500–850+ req/sec under load)  
- Distributed AI systems (RAG, LLM orchestration, vector search)  
- Event-driven architectures (Kafka, async pipelines)  
- API-first platforms for integrations and automation  
- Low-latency systems using caching, batching, and efficient routing  

---

## Flagship System — High-Concurrency AI Platform

Production-grade distributed backend system designed to handle real-world AI workloads at scale.

### Scale

- ~850 req/sec throughput (load-tested)  
- 500+ concurrent requests with stable latency  
- 100K+ documents processed  

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

- ~40% latency reduction  
- ~30% cost reduction  
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
