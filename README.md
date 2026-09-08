# Pharmaceutical Document RAG Prototype

A Retrieval-Augmented Generation (RAG) prototype for extracting, retrieving,
and answering questions from pharmaceutical PDF documents.

This project was developed as part of an AI-powered document extraction
externship. The system supports both digitally generated and scanned PDFs,
retrieves relevant document content, and generates answers with source
citations.

## Features

- PDF text extraction
- OCR for scanned documents
- Table and metadata extraction
- Document chunking
- Semantic vector search
- BM25 keyword retrieval
- Hybrid retrieval
- Cross-encoder reranking
- Metadata-based query routing
- Source citations
- Gradio chatbot interface
- Structured JSON output
- Evaluation of embedding models, chunking strategies, retrieval settings,
  and open-source LLMs

## Technologies

- Python
- Google Colab
- LlamaIndex
- Hugging Face
- PyMuPDF
- PaddleOCR
- BM25
- Gradio

## How It Works

1. A PDF document is uploaded.
2. Text is extracted directly from digital PDFs or through OCR for scanned PDFs.
3. Extracted content is divided into chunks and associated with document metadata.
4. The system indexes the document for semantic and keyword-based retrieval.
5. A user submits a question through the chatbot interface.
6. Relevant document chunks are retrieved using hybrid search and reranking.
7. The language model generates an answer using the retrieved context.
8. The response includes citations to the relevant document sources.

## Evaluation

The project includes experiments comparing:

- Different embedding models
- Fixed-length and semantic chunking strategies
- Retrieval configurations
- Reranking approaches
- Open-source language models

The goal was to evaluate how different RAG pipeline configurations affect
retrieval quality, response accuracy, and performance.

## Interface

A Gradio interface allows users to:

- Upload PDF documents
- Ask questions about document contents
- View generated answers with citations
- View structured response information
- Export results as JSON

## Repository Structure

```text
pharmaceutical-document-rag/
├── README.md
└── pharmaceutical_document_rag.ipynb
