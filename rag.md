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

