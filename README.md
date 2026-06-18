# AI-powered-hr-policy-assistant
AI-powered HR policy assistant built with LangChain, OpenAI, FAISS, and Gradio to provide document-grounded answers from company HR policy documents.

# AI-Powered HR Policy Assistant

## Project Overview

The AI-Powered HR Policy Assistant is a Retrieval-Augmented Generation (RAG) application that enables users to ask questions about company HR policies and receive accurate, document-grounded responses.

The solution combines document processing, semantic search, vector databases, Large Language Models (LLMs), and conversational AI techniques to transform static HR policy documents into an intelligent knowledge assistant.

The system analyzes a Nestlé HR Policy document to:

* Answer employee policy questions
* Retrieve relevant policy information
* Provide document-grounded responses
* Improve accessibility of HR knowledge
* Demonstrate enterprise AI applications

## Business Problem

Organizations often maintain lengthy HR policy documents that employees rarely read in full. Finding specific information within these documents can be time-consuming and inefficient.

This project demonstrates how Generative AI and Retrieval-Augmented Generation (RAG) can improve access to organizational knowledge by enabling employees to ask natural language questions and receive immediate, context-aware answers.

## Dataset

Nestlé HR Policy PDF Document

The document contains information related to:

* Employee responsibilities
* Leave policies
* Workplace conduct
* Employee benefits
* Organizational guidelines
* HR procedures

## Technologies Used

### Programming

* Python

### Generative AI

* OpenAI GPT-3.5 Turbo
* Prompt Engineering

### Frameworks

* LangChain

### Document Processing

* PyPDFLoader
* RecursiveCharacterTextSplitter

### Vector Database

* FAISS

### Embeddings

* OpenAI Embeddings

### User Interface

* Gradio

### Environment Management

* Python Dotenv

## Project Workflow

### 1. Environment Configuration

* Loaded environment variables securely using dotenv
* Retrieved OpenAI API credentials

### 2. Document Loading

* Loaded HR policy PDF document using PyPDFLoader
* Converted document pages into LangChain document objects

### 3. Document Chunking

* Split document into smaller text segments
* Configured chunk size and overlap for contextual retrieval

### 4. Embedding Generation

* Generated vector embeddings using OpenAI Embeddings
* Converted text chunks into numerical vector representations

### 5. Vector Database Creation

* Stored embeddings in a FAISS vector database
* Enabled fast semantic similarity search

### 6. Retrieval System

* Created a retriever to identify the most relevant policy sections
* Retrieved top matching document chunks for each query

### 7. Question Answering Pipeline

* Integrated GPT-3.5 Turbo
* Applied prompt engineering techniques
* Combined retrieved context with user questions
* Generated document-grounded responses

### 8. Testing

* Validated the system using multiple HR policy questions
* Verified retrieval accuracy
* Tested response relevance and consistency

### 9. User Interface

* Developed a Gradio chatbot interface
* Enabled users to submit HR-related questions
* Displayed document-grounded responses interactively

## Key Findings

* Document chunking improved retrieval accuracy
* Semantic search successfully identified relevant policy sections
* GPT-3.5 Turbo generated context-aware responses grounded in retrieved content
* FAISS provided efficient vector similarity search
* The RAG architecture reduced the likelihood of hallucinated responses

## Business Impact

Organizations can use this solution to:

* Improve employee access to HR information
* Reduce repetitive HR inquiries
* Increase productivity through self-service support
* Enhance enterprise knowledge management
* Deploy AI-powered internal assistants

## Project Limitation

Due to environment restrictions and dependency conflicts, the Gradio interface could not be fully deployed within the notebook environment. The retrieval and question-answering pipeline was successfully validated through direct function testing.

## Future Improvements

* Upgrade to GPT-4 models
* Support multiple HR policy documents
* Deploy to cloud infrastructure
* Implement authentication and role-based access
* Integrate enterprise knowledge bases

## Author

Abiodun Sleek
