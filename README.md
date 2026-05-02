<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Backend Engineer focused on building distributed systems that hold up under real-world load
</p>

<p align="center">
  850+ req/sec · ~480ms p95 · Async · Kafka · Redis
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

## Overview

I build backend systems that are designed to stay stable under concurrency, scale, and unpredictable traffic.

My focus is on high-throughput architectures using async execution, distributed caching, and event-driven systems. I care about systems that don’t just work in ideal conditions, but continue to perform under stress.

---

## What I Build

- High-concurrency backend systems (500–850+ req/sec under load)  
- Distributed AI systems (RAG pipelines, LLM orchestration, vector search)  
- Event-driven architectures (Kafka, async workers, message queues)  
- API-first platforms for integrations and automation  
- Low-latency systems using caching, batching, and efficient routing  

---

## Flagship System — High-Concurrency AI Platform

Production-grade backend system built to handle real-world AI workloads at scale.

### Scale

- ~850 req/sec throughput (load-tested)  
- 500+ concurrent requests handled reliably  
- 100K+ documents processed  

### Architecture

- Async FastAPI services (stateless, horizontally scalable)  
- Redis distributed caching  
- FAISS vector index for semantic retrieval  
- Kafka-based event pipelines  
- Multi-LLM routing with fallback handling  

### Engineering Decisions

- Stateless services for horizontal scaling  
- Async pipelines for non-blocking execution  
- Cache-first approach to reduce latency and cost  
- Backpressure handling for system stability  
- API-first design for extensibility  

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
