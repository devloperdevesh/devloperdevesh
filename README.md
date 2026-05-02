<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Backend Engineer building distributed systems that remain reliable under real-world load
</p>

<p align="center">
  Built high-concurrency systems handling 850+ req/sec with sub-500ms latency
</p>

<p align="center">
  Distributed Systems · AI Infrastructure · High-Throughput Backend Engineering
</p>

<p align="center">
  Open to remote opportunities and global collaboration
</p>

<p align="center">
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
</p>

---

## Overview

I build backend systems that do not fail under scale, concurrency, and unpredictable traffic.

My work focuses on designing high-throughput, low-latency systems using async architectures, distributed caching, and event-driven pipelines. I prioritize reliability, performance, and cost-efficiency in production-like environments.

Recently, I designed and load-tested systems handling 850+ requests per second with stable latency, using stateless services, Redis caching, and Kafka-based pipelines.

---

## Engineering Snapshot

- 850+ req/sec throughput under load-tested conditions  
- ~480ms p95 latency under concurrent traffic  
- 500+ concurrent requests handled reliably  
- 100K+ documents processed in distributed pipelines  
- ~40% latency reduction through async and caching strategies  
- ~30% infrastructure cost reduction via optimized routing and caching  

---

## What I Build

- High-concurrency backend systems (500–850+ req/sec under load)  
- Distributed AI systems (RAG pipelines, LLM orchestration, vector search)  
- Event-driven architectures (Kafka, async workers, message queues)  
- API-first platforms for integrations and automation  
- Low-latency systems using caching, batching, and efficient request routing  

---

## Flagship System — High-Concurrency AI Platform

Production-grade distributed backend system designed to handle real-world AI workloads at scale.

### Scale

- 850+ req/sec throughput (load-tested)  
- 500+ concurrent requests with stable latency  
- 100K+ documents processed  

### Architecture

- Async FastAPI services (stateless, horizontally scalable)  
- Redis distributed caching layer  
- FAISS vector index for semantic retrieval  
- Kafka-based event-driven pipelines  
- Multi-LLM routing layer with fallback handling  

### Engineering Decisions

- Stateless architecture for horizontal scalability  
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
