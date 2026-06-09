# Law Simplified
![Python](https://img.shields.io/badge/Python-3.12-blue)
![LLM](https://img.shields.io/badge/LLM-Powered-green)
![RAG](https://img.shields.io/badge/RAG-Enabled-orange)
![OCR](https://img.shields.io/badge/OCR-Multilingual-red)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-ff4b4b)
![Status](https://img.shields.io/badge/Status-Completed-success)
## Overview

Law Simplified is an AI-powered legal document intelligence platform designed to make complex legal documents easier to understand and interact with. The system enables users to upload legal documents such as contracts, agreements, notices, offer letters, policies, and other legal paperwork, automatically extracts and analyzes the content, and presents the information in a structured and user-friendly format.

Beyond document analysis, Law Simplified allows users to interact with their documents through a conversational interface, enabling natural language question-answering based solely on the contents of the uploaded document.

---

## Problem Statement

Legal documents are often lengthy, complex, and written using terminology that is difficult for non-legal professionals to understand. Important information such as obligations, deadlines, clauses, parties involved, and potential risks can be easily overlooked.

Traditional document review requires significant time and attention, making it challenging for individuals to quickly understand the implications of a legal document.

Law Simplified addresses this challenge by transforming legal documents into structured insights, simplified summaries, actionable highlights, and an interactive knowledge base.

---

## Key Features

### Document Upload

* Supports PDF documents and scanned document images.
* Handles both digital and image-based legal documents.
* Designed to process documents of varying lengths and formats.

### Multilingual OCR and Text Extraction

* Extracts text from scanned and image-based documents.
* Supports multilingual document processing.
* Utilizes multiple extraction strategies to improve text recovery accuracy.

### Legal Information Extraction

Automatically identifies and extracts important information such as:

* Parties involved
* Important dates and deadlines
* Key clauses
* Rights and responsibilities
* Legal obligations
* Actionable requirements
* Critical document metadata

### Structured Document Analysis

Generates easy-to-consume outputs including:

* Plain-language document summary
* Key highlights
* Important obligations
* Do's and Don'ts
* Critical action items
* Document-specific insights

### Conversational Document Assistant

Users can ask questions directly about their uploaded document.

Examples:

* What are my obligations under this agreement?
* When does this contract expire?
* What penalties are mentioned?
* Is there a termination clause?
* What actions do I need to take?

The assistant retrieves relevant information from the uploaded document and generates contextual responses based on the document content.

---

## System Architecture

```text
User Uploads Document
        │
        ▼
PDF / Scanned Image Processing
        │
        ▼
Multilingual OCR & Text Extraction
        │
        ▼
Legal Information Extraction
        │
        ├── Parties Involved
        ├── Important Dates
        ├── Clauses
        ├── Rights & Obligations
        └── Key Legal Information
        │
        ▼
Document Analysis Engine
        │
        ├── Summary Generation
        ├── Key Highlights
        ├── Do's and Don'ts
        └── Actionable Insights
        │
        ▼
Vector Embedding Generation
        │
        ▼
Document Knowledge Store
        │
        ▼
Interactive Legal Assistant
        │
        ▼
Question Answering Interface
        │
        ▼
Relevant Context Retrieval
        │
        ▼
AI Generated Response
```
<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/99ff3ba7-3b19-4f65-bea2-c7568b1e8fb7" />

---

## Workflow

### Step 1: Document Ingestion

The user uploads a legal document in PDF or image format.

### Step 2: Content Extraction

The system extracts textual content using OCR and document parsing techniques.

### Step 3: Legal Information Analysis

The extracted content is analyzed to identify important legal entities, obligations, dates, clauses, and other relevant information.

### Step 4: Structured LLM Schema

The document is transformed into simplified summaries and structured outputs that are easier to understand than the original legal text.

### Step 5: Vector Embedding 

The processed document is converted into vector embeddings and stored within a temporary document-specific knowledge store.

### Step 6: Interactive Interaction

Users can ask questions regarding the uploaded document. Relevant sections are retrieved from the document knowledge base and used to generate context-aware responses.

---
### Document Type
Employment Agreement

### Parties Involved
- ABC Technologies Pvt Ltd
- John Doe

### Important Dates
- Employment Start Date: 01 January 2025
- Notice Period: 90 Days

### Key Obligations
- Maintain confidentiality
- Follow company policies
- Avoid conflicts of interest

### Important Clauses
- Confidentiality Clause
- Non-Compete Clause
- Termination Clause

### Simplified Summary
This agreement outlines the employment relationship, compensation structure, employee responsibilities, confidentiality requirements, and termination conditions.
Mentions : Do's:
         : Do Not's:
---


## Sample Analysis Output

```json
{
  "document_type": "Employment Agreement",
  "parties": [
    "ABC Technologies Pvt Ltd",
    "John Doe"
  ],
  "effective_dates": {
    "start_date": "01 January 2025",
    "notice_period": "90 Days"
  },
  "payment_terms": "Monthly salary payable on the last working day of each month.",
  "termination_or_expiry": "Agreement may be terminated with 90 days written notice.",
  "key_obligations": [
    "Maintain confidentiality",
    "Follow company policies",
    "Avoid conflicts of interest"
  ],
  "important_clauses": [
    "Confidentiality Clause",
    "Non-Compete Clause",
    "Termination Clause"
  ],
  "simplified_summary": "This agreement defines employment terms, compensation, confidentiality obligations, and termination conditions."
  Do's: Mention list of Important and must required tasks to be done by user 
  Do Not's: Must not violate key obligations etc etc 
}
```
---

## Technology Stack

### Backend

* Python

### AI & NLP

* Large Language Models (LLMs)
* Retrieval-Augmented Generation (RAG)
* Embedding Models
* Prompt Engineering

### Document Processing

* PDF Parsing
* Optical Character Recognition (OCR)
* Multilingual Text Extraction

### Search & Retrieval

* Vector Embeddings
* Semantic Search
* Similarity-Based Retrieval

### Frontend

* Streamlit

---

## Design Principles

### Document-Centric Processing

Every uploaded document is treated independently, ensuring that responses remain focused on the specific document being analyzed.

### Simplified Legal Understanding

Outputs are designed for non-legal users, prioritizing clarity and accessibility over legal jargon.

### Retrieval-Based Question Answering

The conversational assistant references information extracted from the uploaded document to improve relevance and consistency of responses.

### Temporary Knowledge Base

Document embeddings are generated for the uploaded document session and used exclusively for that document's analysis and interaction workflow.

---

## Challenges Addressed

### Complex Legal Language

Transforms dense legal content into understandable summaries and structured insights.

### Scanned Document Processing

Supports image-based legal documents through OCR-enabled text extraction.

### Information Discovery

Reduces the effort required to locate important clauses, dates, and obligations.

### Document Navigation

Enables users to interact with lengthy documents through natural language questions instead of manual searching.

---

## Future Enhancements

* Multi-document comparison
* Clause-level document comparison
* Risk assessment indicators
* Legal document classification
* Cross-document knowledge retrieval
* Advanced citation and source tracking
* Support for additional legal document categories

---

## My Contribution

This project was independently conceptualized, designed, and developed end-to-end.

Areas of contribution include:

* System architecture design
* Legal document processing workflow
* OCR integration strategy
* Information extraction pipeline
* Retrieval-Augmented Generation workflow
* Embedding and retrieval design
* Prompt engineering
* Frontend development
* Testing and evaluation

---
