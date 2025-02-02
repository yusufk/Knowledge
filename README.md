# LightRAG Experiment

Testing the lightweight RAG System on local setup using Ollama for local LLM operations.

## Overview

This project demonstrates a lightweight RAG system using two Jupyter notebooks:

* `lightrag-ingestion-notebook.ipynb` - Handles document processing and embedding generation
* `lightrag-query-notebook.ipynb` - Implements querying and response generation

## Features

* Fully local RAG implementation using Ollama
* Uses nomic-embed-text for embeddings
* Supports PDF and text document ingestion
* Chunking with configurable overlap
* Vector similarity search for relevant context retrieval
* Flexible LLM model selection for response generation

## Prerequisites

* Python 3.x
* Ollama installed and running locally
* Required Ollama models:
  * `nomic-embed-text` (for embeddings)
  * Your choice of LLM (e.g., `llama2`, `deepseek-r1:8b`)

## Usage

1. Pull and start required Ollama models:
   ```bash
   ollama pull nomic-embed-text
   ollama pull deepseek-r1:8b

2. Verify that the models are running:
   ```bash
   ollama list
   ```

3. Run the ingestion notebook to process documents and generate embeddings:
   ```bash
   jupyter notebook lightrag-ingestion-notebook.ipynb
   ```

4. Run the query notebook to query the processed documents and generate responses:
   ```bash
    jupyter notebook lightrag-query-notebook.ipynb
    ```