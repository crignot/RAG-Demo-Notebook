# Retrieval-Augmented Generation (RAG) Demo Notebook

This repository contains a Jupyter notebook which implements a small end-to-end **retrieval-augmented generation (RAG)** pipeline as a personal learning project.

This notebook builds a small end-to-end RAG pipeline that:
- Scrapes selected CS 61B course pages using Firecrawl  
- Splits the scraped text into overlapping chunks  
- Embeds and stores chunks in a Pinecone vector database  
- Retrieves the relevant chunks for a user query  
- Generates grounded answers using Google Gemini, with source URLs returned for traceability  

This project was built as a **personal learning exercise and preparation** for working with RAG-based systems. The focus was on understanding the full RAG workflow and the role of retrieval and source grounding, rather than building a production-ready system.

## Notes
- API keys are expected to be provided via environment variables and are not included in this repository.
- The Pinecone index is rebuilt by default for a clean demo run (this behavior can be changed in the notebook).
