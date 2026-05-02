<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Building distributed systems handling <b>850+ req/sec</b> with sub-500ms latency
</p>

<p align="center">
  FastAPI · Redis · Kafka · Async Systems · AI Infrastructure
</p>

<p align="center">
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">LinkedIn</a>
</p>

---

## Engineering Activity

<p align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=devloperdevesh&show_icons=true&theme=default&hide_border=true&bg_color=ffffff" height="160"/>
  <img src="https://streak-stats.demolab.com?user=devloperdevesh&theme=default&hide_border=true&background=ffffff" height="160"/>
</p>

---

## Open Source

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=devloperdevesh&theme=github&bg_color=ffffff&color=111827&line=2563eb&point=2563eb&area=true&hide_border=true" width="85%"/>
</p>

<p align="center">
  <sub>Consistent contributions across backend systems and AI infrastructure</sub>
</p>

---

## What I Build

- High-concurrency backend systems (500–850+ req/sec)
- Distributed AI systems (RAG, LLM orchestration, vector search)
- Event-driven architectures (Kafka, async pipelines)
- Low-latency APIs using caching, batching, and routing

---

## Flagship System — High-Concurrency AI Platform

Production-grade backend system designed for real-world AI workloads.

### Scale

- ~850 req/sec throughput  
- 500+ concurrent requests  
- 100K+ documents processed  

### Architecture

- Stateless FastAPI services  
- Redis caching layer  
- FAISS-based retrieval  
- Kafka event pipelines  
- Multi-LLM routing  

### Impact

- ~40% latency reduction  
- ~30% cost reduction  
- Stable under sustained and burst traffic  

---

## System Architecture

```mermaid
graph TD
    Client --> CDN
    CDN --> LB
    LB --> API
    API --> Redis
    API --> Workers
    Workers --> FAISS
    FAISS --> LLM
    LLM --> Response
