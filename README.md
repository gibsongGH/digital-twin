# Greg's Digital Twin
> Live demo available on Hugging Face Spaces:  [Digital Twin](https://huggingface.co/spaces/gibsongHF/digital-twin)

An AI-powered digital twin that answers questions about my professional background using my own documents and project history.

Built as a practical application of Retrieval-Augmented Generation (RAG), this project turns static career materials into a searchable, conversational system.

## Overview

This application allows users to ask natural language questions about my experience, skills, and projects. Instead of relying on generic model knowledge, responses are grounded in curated personal documents.

It’s essentially a structured, queryable version of a resume — with context.

## What it can do

- Answer questions about my work history and roles
- Explain projects and technical decisions
- Summarize skills and tools across different domains
- Retrieve relevant context from source documents
- Generate clear, conversational responses based on that context

## Why I built it

I wanted to move beyond static portfolios and build something interactive that demonstrates how AI systems actually work.

This project reflects how I think about AI engineering:
- structured inputs
- controlled retrieval
- explainable outputs
- real-world usefulness over novelty

## How it works

1. Personal documents are chunked and embedded
2. Embeddings are stored in a vector database
3. User queries are converted into embeddings
4. Relevant chunks are retrieved
5. An LLM generates a response using that context

## Tech stack

- Python
- Gradio (UI)
- OpenAI API (LLM + embeddings)
- Vector database (Chroma or similar)
- dotenv for configuration

## Running locally

git clone <your-repo-url>
cd digital-twin
python -m venv venv
venv\Scripts\activate   # Windows
pip install -r requirements.txt

Create a .env file:
OPENAI_API_KEY=your_key_here
OPENAI_PROJECT_ID=your_project_id

Run the app:
python app.py

## Project notes

This is an evolving project as I continue building toward more advanced AI systems, including tool use, orchestration, and multi-step reasoning workflows.

## Links
- Hugging Face Space: [Live demo](https://huggingface.co/spaces/gibsongHF/digital-twin)
- Portfolio: [Website](https://gibson-ai.com)
