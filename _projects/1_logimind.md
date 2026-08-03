---
layout: page
title: LogiMind
description: Multi-agent RAG system for querying public logistics operational data in natural language
img:
importance: 1
category: ai
---

LogiMind is a multi-agent Retrieval-Augmented Generation (RAG) system that lets you query a public logistics knowledge base in natural language and get grounded, cited answers back instead of a wall of documents.

The system is built around a team of cooperating agents — orchestrated with **AutoGen** and **LangChain** — that split a query into sub-tasks, retrieve relevant context from a **Qdrant** vector store, and synthesize a final answer. Retrieval quality and answer faithfulness are continuously evaluated with **RAGAS**, and every run is traced end-to-end with **LangSmith** so regressions in retrieval or generation are caught before they reach a user. The system is served through a **FastAPI** backend with a **Streamlit** front end, deployed on **AWS**.

This is my flagship project for the transition from data engineering into AI/LLM engineering: it applies the same rigor I used to bring to data pipelines — testability, observability, evaluation — to an agentic RAG system instead of a batch ETL job.

**Stack:** AutoGen, LangChain, RAGAS, LangSmith, Qdrant, FastAPI, Streamlit, AWS

**Status:** In active development

**Code:** [github.com/awais-de/logimind](https://github.com/awais-de/logimind)
