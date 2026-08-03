---
layout: page
title: LogiMind
description: Multi-agent RAG over public logistics operational documentation
img:
importance: 1
category: ai
---

Multi-agent RAG system for querying public logistics operational documentation in natural language.

A fixed-orchestration agent pipeline — planner, retriever, responder — runs hybrid BM25 and dense retrieval against a **Qdrant** vector store, served through a **FastAPI** backend with a **Streamlit** UI. The pipeline is instrumented end to end with **LangSmith** tracing and evaluated continuously with **RAGAS**.

**Measured:** 0.98 faithfulness, ~9.4s median latency, $0.028 per query. 108 tests, Dockerized, CI on every push, deployed live.

Architectural decisions are documented in the repo — including why the retriever agent is deliberately not LLM-backed, and why I chose fixed orchestration over an AutoGen group chat.

**Stack:** AutoGen, LangChain, Qdrant, RAGAS, LangSmith, FastAPI, Streamlit, hybrid BM25 + dense retrieval, Docker, GitHub Actions, AWS

**Status:** Deployed, CI on every push

**Code:** [github.com/awais-de/logimind](https://github.com/awais-de/logimind)
