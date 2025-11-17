# rag_evaluation_pipeline

📌 Overview

This repository contains a simple yet powerful RAG (Retrieval-Augmented Generation) evaluation pipeline using:

LlamaIndex for indexing & retrieval

Local GGUF LLMs (no API key required)

HuggingFace embeddings

BLEU, ROUGE, Cosine Similarity for evaluation

The project demonstrates how to evaluate LLM answers against ground truth using multiple metrics—ideal for ML engineering interviews, learning purposes, and research experiments.

⭐ Features
🔍 Retrieval-Augmented Generation (RAG)

Indexes a document (sample medical text on cancer)

Retrieves relevant chunks using embeddings

Sends context + question to a local LLM

🧠 Local LLM Inference (No API Key Needed)

Uses a GGUF model like:

Mistral-7B-Instruct-Q4_K_M.gguf

Works fully offline

Runs on CPU/GPU depending on the environment

📊 Evaluation Metrics

The pipeline evaluates model performance using:

Metric	Purpose
Cosine Similarity	Semantic similarity between answer & GT
BLEU Score	Measures wording/pattern overlap
ROUGE-1 / ROUGE-L	Measures recall & phrasing similarity

| Question        | Cosine | BLEU | ROUGE-1 | ROUGE-L |
| --------------- | ------ | ---- | ------- | ------- |
| What is cancer? | 0.944  | 0.13 | 0.38    | 0.38    |
| Symptoms?       | 0.813  | 0.09 | 0.32    | 0.30    |
| Spread?         | 0.922  | 0.11 | 0.36    | 0.34    |



