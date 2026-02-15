# 🏗️ PrepOS: Technical Design Document
> **Architecture & Implementation Blueprint**

---

## 1. 🖼️ Design Overview
PrepOS is designed as a modular, session-first application. It prioritizes data integrity and fast retrieval for the AI "Second Brain" functionality.

---

## 2. 🏛️ System Architecture

### 🔄 The High-Level Flow
1.  **Frontend:** Next.js (React) for a snappy, IDE-like experience.
2.  **Backend:** Django REST Framework for robust API management and ORM.
3.  **Database:** PostgreSQL for relational data; Vector DB for AI context.
4.  **AI Layer:** OpenAI/Anthropic APIs for note generation and RAG.

---

## 3. 📊 Architecture Diagram

```mermaid
graph TD
    User((User)) -->|Interacts| FE[Next.js Frontend]
    
    subgraph "Application Layer"
        FE -->|API Calls| BE[Django REST Backend]
        BE -->|Auth/Data| DB[(PostgreSQL)]
    end

    subgraph "AI & Processing"
        BE -->|Context| AI{AI Processing Engine}
        AI -->|LLM| GPT[OpenAI / Anthropic]
        AI -->|Embeddings| VDB[(Vector Database)]
    end

    subgraph "Special Modules"
        FE -->|Visuals| SDH[System Design Hub]
        BE -.->|Future| SBX[Docker Sandbox]
    end

    GPT -->|Notes/Tags| BE
    VDB -->|Search Results| BE
