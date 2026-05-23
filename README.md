# Brian Jackson

AI Engineer & Consulting Architect with 11+ years building enterprise **search,
analytics, and agentic AI platforms** — currently delivering Elastic solutions
to Fortune 500 clients while pursuing an MS in Data Science (AI/ML) at Texas
Tech.

My core is search and retrieval at scale — Elasticsearch, hybrid/semantic
search, RAG, multi-modal — and I build LLM features the way they have to work in
production: the model is one component in an engineered system, not the whole
system. That means schema-bound output, deterministic verification, safety
screening, graceful degradation, and cost guardrails — not just a prompt and a
hope.

## What I work on

**Search & retrieval at scale** — Hybrid semantic search (BM25 + KNN + RRF),
ESRE, ELSER/E5 embeddings, relevance tuning, cross-cluster replication, and
cluster/shard architecture on Elasticsearch 8.x/9.x for Fortune 500 workloads.

**Applied LLM systems** — RAG, prompt systems with safety guardrails,
deterministic output validation, multi-agent orchestration, and cost-bounded
model routing. On-prem and cloud inference (Anthropic Claude, OpenAI, local
models via Ollama/LiteLLM).

## Selected public work

**[bj-structured-llm-extraction](https://github.com/jacksobk/bj-structured-llm-extraction)** — Structured extraction from freeform text with a deterministic verification layer.
The model proposes a structured result; non-LLM code validates the schema and
applies business policy (e.g. high-stakes intents are always routed to human
review, regardless of model confidence). Includes a prompt-injection screen and
corrective-retry on invalid output. *TypeScript · NestJS · tested · CI.*

**[bj-llm-gateway-cost-guard](https://github.com/jacksobk/bj-llm-gateway-cost-guard)** — An LLM gateway with tiered routing and a hard cost guardrail.
Cheap-model-first, escalates to a stronger model only on error or low
confidence, and enforces a monthly budget cap that degrades gracefully instead
of running up a surprise bill. Every response shows which tier served it and
what it cost. *TypeScript · NestJS · tested · CI.*

**[FindWaldo](https://github.com/jacksobk/FindWaldo)** — Multimodal visual search.
Vector search over image embeddings (Jina CLIP v2) with an evaluation harness —
IoU metrics, per-category success rates — for tuning retrieval relevance.
*Python.*

**[bj-backend-member](https://github.com/jacksobk/bj-backend-member)** — A layered microservice reference implementation: strict layer separation, an endpoint registry as a single source of truth, a standardized response envelope, and per-request structured logging. *TypeScript · NestJS.*

## Focus areas

Search & retrieval at scale · RAG / hybrid / semantic / multi-modal search ·
LLM integration & output validation · prompt systems & safety guardrails ·
multi-agent orchestration · API & microservice architecture · Elastic Stack.

## Certifications

Elastic Certified Engineer · Elastic Certified Observability Engineer · Elastic
Certified Data Analyst (2025)
