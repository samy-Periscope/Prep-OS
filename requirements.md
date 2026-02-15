# 💻 PrepOS: Requirement Document
> **Preparation Operating System** — *The Continuous Learning Loop for DSA.*

---

## 1. 🎯 Introduction
**PrepOS** is a personal operating system for DSA preparation that combines executable code, auto-generated notes, daily sessions, task accountability, and AI-driven reflection into one seamless workflow.

The goal of this system is to bridge the gap between **solving** a problem and **retaining** the underlying logic.

---

## 2. ⚠️ Problem Statement
PrepOS solves 5 intertwined problems that traditional platforms ignore:

### 🧠 2.1 Fragmented Learning Memory
* **The Gap:** Code is on LeetCode, notes are in Notion, and progress is "in your head."
* **The Fix:** A single session-based memory system where code, notes, links, and reflections coexist.

### 📝 2.2 Code Without Conceptual Retention
* **The Gap:** You solve a problem today but forget the "aha!" moment in 2 weeks.
* **The Fix:** AI-driven structured notes generated directly from your code and comments.

### 📉 2.3 No Quality Feedback Loop
* **The Gap:** Most tools track *quantity* (problems solved) but ignore *quality* (weakness patterns).
* **The Fix:** A reflective loop identifying repeating concepts and avoided topics.

### 🤝 2.4 Lack of Accountability
* **The Gap:** To-do apps are too easy to ignore.
* **The Fix:** Non-negotiable tasks + AI "mentor" check-ins to maintain momentum.

### 🕸️ 2.5 No "Second Brain" for DSA
* **The Gap:** Learners don't build a searchable knowledge graph of their own journey.
* **The Fix:** A tag-based, AI-queryable archive of every logic gate you've ever built.

---

## 3. 👥 Target Users
* **🎓 CS Students:** Preparing for high-stakes placements and internships.
* **🏆 Competitive Programmers:** Focusing on contest performance and rating growth.
* **⚡ Self-driven Learners:** Building a long-term technical "Second Brain."

---

## 4. ⚙️ Functional Requirements

### 📅 4.1 Daily Session System (Core Unit)
* **Create Session:** Daily containers for focused prep.
* **Data Aggregation:** Each session bundles questions, snippets, and reflections.
* **Metadata:** Tracks date, volume, concepts, and completion status.

### 🖥️ 4.2 Code Workspace
* **Multi-Lang:** C++, Java, Python (Phase 1); JS, Go (Phase 2).
* **Intellisense:** Syntax highlighting and versioned saves.
* **Conversion Engine:** AI logic to port code between languages while keeping comments intact.

### 🤖 4.3 AI Notes Generator
* **Trigger:** One-click "Generate Notes" from active code.
* **Output:** Structured summaries, time complexity analysis, and "Key Takeaways."

### 🏷️ 4.4 Smart Tagging
* **Auto-Detect:** AI detects `Array`, `DP`, `Backtracking` etc.
* **Organization:** Enables deep search and concept-based analytics.

### 🔗 4.5 Link Association
* **Vault:** Attach YouTube tutorials, LeetCode links, or PDFs to specific sessions.

### 🚀 4.6 Task Management
* **Non-Negotiables:** Tasks that directly impact your "Streak" health.
* **Context Aware:** Tasks are linked to sessions for historical tracking.

### 📊 4.7 Profile & Analytics
* **Heatmaps:** Daily/Weekly prep intensity.
* **Skill Radar:** Visualizing strengths (e.g., strong in Strings, weak in Graphs).

### 💬 4.8 AI Chatbot (RAG-Based)
* **Context:** Knows your history. Ask: *"What DP problems did I struggle with last week?"*
* **Role:** Acts as a Mentor, Reflector, and Study Planner.

### 🏛️ 4.9 System Design Learning Hub
* **Simulations:** Interactive visualizers for Caching, Load Balancing, and Sharding.

---

## 5. 🛡️ Non-Functional Requirements
* **⚡ Performance:** Instant editor response; lazy-loaded analytics.
* **🔒 Security:** Private-by-default data; secure sandbox for code (Phase 2).
* **📈 Scalability:** Vector DB integration for fast AI retrieval.

---

## 6. 🚧 Constraints & Assumptions
* **Phase 1:** Web-focused MVP.
* **Code Exec:** Initial release focuses on storage and AI notes; execution is Phase 2.
