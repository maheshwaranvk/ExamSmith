# 🧠 ExamSmith

## AI-Powered Exam Question Generation Platform (RAG-Based) 🚀

------------------------------------------------------------------------

# 📌 Overview

ExamSmith is a production-ready AI-powered exam question generation
system built using a Retrieval-Augmented Generation (RAG) architecture.

It ingests textbooks, requirement documents, and past/model question
papers, converts them into embeddings, retrieves relevant academic
context, and generates structured, exam-aligned questions using Large
Language Models (LLMs).

The system is modular, scalable, evaluation-driven, and designed for
real-world academic environments.

------------------------------------------------------------------------

# 🚨 Problem Statement

Traditional exam paper creation is:

-   Manual and repetitive\
-   Time-consuming\
-   Highly dependent on individual expertise\
-   Difficult to standardize\
-   Hard to validate for coverage

Educators must repeatedly analyze textbooks and past question papers
while ensuring syllabus alignment and difficulty balance.

------------------------------------------------------------------------

# 💡 Solution Approach

ExamSmith solves this using:

-   Context-aware retrieval instead of blind generation\
-   Hybrid Search (BM25 + Semantic Vector Search)\
-   Structured output validation\
-   Evaluation-driven generation\
-   Modular backend services

The system ensures questions are grounded in real academic content
rather than hallucinated responses.

------------------------------------------------------------------------

# 🏗 System Architecture

ExamSmith follows a layered architecture:

1.  Frontend (React-based Web UI)\
2.  Backend APIs (FastAPI services)\
3.  Injection Layer (Data Processing & Embeddings)\
4.  Retrieval & Generation Layer (Hybrid RAG)\
5.  Storage Layer (MongoDB + Vector Database)\
6.  Evaluation & Observability Layer

------------------------------------------------------------------------

# 🔄 End-to-End Workflow

## 📥 Phase 1: Data Injection (Offline)

1.  Upload textbooks, requirement docs, or past question papers\
2.  Text cleaning & normalization\
3.  Intelligent chunking strategy\
4.  Embedding generation\
5.  Metadata tagging\
6.  Storage in MongoDB + Vector DB

## 📤 Phase 2: Question Generation (Online)

1.  User submits a query (e.g., "Generate 10-mark questions")\
2.  Hybrid retrieval fetches relevant chunks\
3.  Re-ranking improves relevance\
4.  Deduplication removes overlaps\
5.  Context summarization optimizes token usage\
6.  Prompt orchestration prepares structured input\
7.  LLM generates questions\
8.  Schema validation ensures structured output\
9.  Evaluation pipeline checks faithfulness & grounding\
10. Output returned to UI

------------------------------------------------------------------------

# 🧠 Retrieval Strategy

### 📘 Textbooks

-   Hybrid Search (BM25 + Vector Search)
-   Metadata filtering
-   Chunk-level semantic retrieval

### 📝 Question Papers

-   Vector-only retrieval
-   Semantic similarity scoring

------------------------------------------------------------------------

# 🔍 Post-Retrieval Pipeline

-   Re-ranking of retrieved chunks\
-   Semantic deduplication\
-   Context compression & summarization\
-   Structured prompt injection\
-   JSON schema validation

------------------------------------------------------------------------

# 📊 Evaluation Framework

ExamSmith integrates evaluation mechanisms to measure:

-   Faithfulness\
-   Hallucination detection\
-   Context precision\
-   Context recall\
-   Output relevancy\
-   Structured format compliance

Evaluation results are stored in JSON format for analysis.

------------------------------------------------------------------------

# 🔐 Authentication & Security

-   JWT-based authentication\
-   Password hashing\
-   Role-ready architecture (Admin / Instructor / Student)\
-   Secure API communication

------------------------------------------------------------------------

# 🗂 Repository Structure

ExamSmith/ ├── Frontend/\
├── backend/\
│ ├── injection/\
│ ├── retrival/\
│ ├── common/\
│ ├── config/\
├── data/\
│ ├── raw/\
│ ├── processed/\
│ ├── evaluation/\
├── docs/\
└── README.md

------------------------------------------------------------------------

# 🛠 Tech Stack

## Backend

-   Python\
-   FastAPI

## AI / NLP

-   Large Language Models (LLMs)\
-   Embedding Models\
-   Retrieval-Augmented Generation (RAG)\
-   Hybrid Search (BM25 + Vector)

## Database

-   MongoDB\
-   Vector Database

## Frontend

-   React\
-   JavaScript

------------------------------------------------------------------------

# 🌟 Key Features

-   AI-driven contextual understanding\
-   Hybrid retrieval pipeline\
-   Modular microservice-style backend\
-   Evaluation-driven generation\
-   Schema-validated structured outputs\
-   Secure authentication\
-   Production-ready architecture

------------------------------------------------------------------------

# 🎯 Target Users

-   Teachers & Professors\
-   Schools & Universities\
-   EdTech Platforms\
-   Students for practice & revision

------------------------------------------------------------------------

# 🚀 Future Enhancements

-   Role-based access control (RBAC)\
-   Difficulty tuning (Easy/Medium/Hard)\
-   PDF export of question papers\
-   Multi-language support\
-   Advanced analytics dashboard\
-   Performance & cost monitoring

------------------------------------------------------------------------

# 🏁 Final Summary

ExamSmith is a scalable, modular, and evaluation-driven AI platform that
transforms academic content into structured, exam-ready question papers
using a Hybrid RAG architecture.

It replaces manual exam creation workflows with intelligent,
context-aware AI generation.
