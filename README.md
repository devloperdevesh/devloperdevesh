<h1 align="center">Devesh Chauhan</h1>

<p align="center">
  Building distributed systems handling <b>850+ req/sec</b> with sub-500ms latency
</p>

<p align="center">
  Async • Kafka • Redis • Low-Latency APIs • AI Infrastructure
</p>

<p align="center">
  <a href="https://linkedin.com/in/devesh-chauhan-6b5691308">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
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
  <img 
    src="https://github-readme-activity-graph.vercel.app/graph?username=devloperdevesh&theme=github&bg_color=ffffff&color=0f172a&line=3b82f6&point=2563eb&area=true&area_color=e0f2fe&hide_border=true"
    width="85%"
  />
</p>

<p align="center">
  <sub><b>Consistent contributions • Performance-focused systems • Built in public</b></sub>
</p>

---

## What I Build

- High-concurrency backend systems (**500–850+ req/sec**)  
- Distributed AI systems (**RAG, LLM orchestration, vector search**)  
- Event-driven architectures (**Kafka, async pipelines**)  
- Low-latency APIs using caching, batching, and routing  

---

## Flagship System — High-Concurrency AI Platform

**Production-grade distributed backend for AI workloads**

### ⚡ Scale
- ~850 req/sec throughput  
- 500+ concurrent users  
- 100K+ documents processed  

### 🧠 Architecture
- Async FastAPI services (stateless)  
- Redis caching layer  
- FAISS vector search  
- Kafka event pipelines  
- Multi-LLM routing  

### 📈 Impact
- ↓ ~40% latency  
- ↓ ~30% cost  
- Stable under burst traffic  

---

## System Architecture

```mermaid
graph TD
    Client --> CDN
    CDN --> LB[Load Balancer]
    LB --> API[FastAPI Gateway]
    API --> Cache[Redis]
    API --> Workers
    Workers --> VectorDB[FAISS]
    VectorDB --> LLM
    LLM --> Response
