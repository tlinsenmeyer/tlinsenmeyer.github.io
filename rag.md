---
layout: home
title: "Developing RAG"
---


# RAG System with LangChain and Chroma

This project built a retrieval‑augmented generation (RAG) pipeline to answer questions about Grok AI using only Wikipedia context.

---

## What I Did

- Loaded Wikipedia content using LangChain  
- Split text into chunks using a recursive splitter  
- Created embeddings with OpenAI  
- Stored vectors in ChromaDB  
- Built a retriever + LLM pipeline  
- Queried the system to validate accuracy  

---

## Tools Used

- LangChain  
- ChromaDB  
- OpenAI Embeddings  
- ChatOpenAI  
- Python  

---

## Key Findings

- RAG improves accuracy by grounding responses in retrieved text  
- LangChain’s newer APIs differ significantly from older tutorials  
- Chroma automatically persists embeddings  
- RAG works well for small datasets but struggles at scale  

---

## Why This Project Matters

RAG is becoming a standard approach for enterprise AI systems. This project shows how retrieval can improve reliability and reduce hallucinations.

[View this Project Notebook (via nbviewer)](https://nbviewer.org/github/tlinsenmeyer/Rag_with_Langchain/blob/main/rag_with_langchain.ipynb)

---

<p align="center" style="color:#C0C0C0; font-size: 0.9em;">
  <span style="color:#00AEEF;">●</span>
  Engineering • Simulation • Machine Learning
  <span style="color:#00AEEF;">●</span><br>
  <span style="color:#2EC4B6;">Designing Smarter Systems</span><br><br>
  <span style="color:#777777;">© 2026 Tom Linsenmeyer</span>
</p>


