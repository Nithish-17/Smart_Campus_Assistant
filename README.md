# Smart_Campus_Assistant
AI-powered study assistant that uses RAG to answer questions, summarize notes, and generate quizzes from student-uploaded documents using Java and Spring Boot.

## 🧩 Problem Statement

College students often face challenges such as:
- Scattered lecture notes across multiple PDFs and documents
- Difficulty finding specific answers inside long materials
- Time-consuming manual revision before exams
- Lack of effective self-assessment tools

There is a need for an intelligent system that can **understand academic documents**, provide **precise answers**, and help students **revise effectively**.

---

## 🎯 Project Overview

**Smart Campus Assistant** solves this problem by acting as an AI-powered educational assistant that:

- Converts uploaded study materials into a searchable knowledge base
- Answers student questions using **Retrieval-Augmented Generation (RAG)**
- Summarizes lengthy documents into concise explanations
- Generates quizzes to improve learning and retention

The system ensures that AI responses are **based only on the student’s uploaded content**, reducing hallucinations and improving accuracy.

---

## 👥 User Roles

### 👨‍🎓 Student
- Upload study materials
- Ask questions in natural language
- View summaries and generated quizzes
- Track learning and revision progress

### 🧑‍💼 Admin (Optional / Future)
- Manage users and documents
- Monitor system usage
- Upload shared academic materials

---

## ✅ Core Features / Functionality

### 📂 Document Management
- Upload PDFs, PPTs, DOCX files
- Automatic text extraction using PDF parsing
- Chunking and indexing of content

### 🤖 AI Question & Answer (RAG)
- Natural language Q&A
- Answers generated strictly from uploaded materials
- Context-aware and source-based responses
- Safe fallback when information is not available

### 📝 Summarization
- Short and detailed summaries
- Key-point extraction for quick revision

### 🧪 Quiz & Practice
- MCQ generation
- Short-answer questions
- Answer explanations for better understanding

### 🔐 Security
- User authentication using JWT
- Secure API access via Spring Security
- User-specific document isolation
- Secure file upload handling

### 📑 API Documentation
- Interactive API documentation using Swagger UI
- Easy testing and validation using Postman

---

## 🧠 How RAG Works in This Project

1. User uploads study materials  
2. Text is extracted and split into smaller chunks  
3. Each chunk is converted into an embedding  
4. Embeddings are stored in PostgreSQL using **pgvector**  
5. User query is embedded and matched using vector similarity  
6. Most relevant chunks are retrieved  
7. Retrieved context is sent to the LLM  
8. AI generates a precise, context-based response  

---

## 🧱 Technologies Used

| Layer / Component       | Technology / Framework |
|------------------------|------------------------|
| Programming Language   | Java 17+ |
| Backend Framework      | Spring Boot |
| Security               | Spring Security + JWT |
| Database               | PostgreSQL |
| Vector Storage         | pgvector (PostgreSQL extension) |
| AI / RAG Integration   | Spring AI / LangChain4j + LLM APIs |
| Document Processing   | Apache PDFBox (or iText) |
| API Docs & Testing    | Swagger UI, Postman |
| Frontend (Optional)   | React + TypeScript + Tailwind OR Thymeleaf |

---

## 📦 Project Structure (Example)


