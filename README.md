# RAG LangGraph Chatbot

An AI-powered question-answering chatbot built using Retrieval-Augmented Generation (RAG) and LangGraph.

The project explores how LLMs can be combined with document retrieval and graph-based workflows to build a more reliable and structured conversational system.

## Overview

Large Language Models can generate useful responses, but they may not have access to private or domain-specific information.

This project uses a RAG pipeline to retrieve relevant information and provide it to the LLM as context before generating a response.

LangGraph is used to structure the application as a workflow, making it easier to control how retrieval, reasoning, and response generation happen.

## Architecture

The high-level flow is:

User Query
    ↓
Query Processing
    ↓
Retriever
    ↓
Relevant Documents
    ↓
LLM + Retrieved Context
    ↓
Response Generation
    ↓
User


The application is organized around the following components:

- `ingest.py` - Handles document ingestion and preparation.
- `agent.py` - Defines the LangGraph/agent workflow and chatbot logic.
- `app.py` - Application entry point.
- `experiments.ipynb` - Used for experimentation and testing during development.

## Key Features

- Retrieval-Augmented Generation (RAG)
- LangGraph-based workflow orchestration
- Context-aware question answering
- Document ingestion and retrieval
- LLM-powered response generation
- Modular Python implementation
- Experimentation through Jupyter Notebook

## Tech Stack

- Python
- LangGraph
- LangChain
- Large Language Models (LLMs)
- Retrieval-Augmented Generation (RAG)
- Vector Embeddings
- Vector Search
- Jupyter Notebook

## Project Structure

```text
RAG_Langgraph_chatbot/
│
├── agent.py              # LangGraph agent/workflow
├── app.py                # Application entry point
├── ingest.py             # Document ingestion pipeline
├── experiments.ipynb     # Experiments and development
├── pyproject.toml        # Project dependencies/configuration
├── uv.lock               # Locked dependencies
└── README.md             # Project documentation
