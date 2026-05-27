# AI-Native Diagnostic & Intelligence Platform

A high-performance, distributed backend system designed to provide real-time, AI-driven insights into complex system logs and operational data.

## 🌟 Why "AI-Native"?
Unlike traditional monitoring that relies on hard-coded thresholds, this platform is built with a **probabilistic reasoning layer**. The AI is not a "bolt-on" feature; it is the core engine that interprets unstructured system data to provide human-readable solutions.

## 🛠 Tech Stack
- **Infrastructure:** FastAPI (Asynchronous Backend), Apache Kafka (Stream Processing)
- **AI Core:** LangChain, OpenAI/Llama-3, ChromaDB (Vector Store)
- **Data & Cache:** Redis (Metadata Caching), SQLite (Local Persistence)

## ⚙️ Core Workflow
1. **Stream:** Logs are pushed through Kafka topics.
2. **Retrieve:** Relevant diagnostic context is fetched from the Vector Database using semantic search.
3. **Reason:** An AI Agent analyzes the log + context to predict the root cause.
4. **Deliver:** Real-time fixes are delivered via REST API/WebSockets.

## 🚦 Getting Started
1. Clone the repo.
2. Run `pip install -r requirements.txt`.
3. Add your `OPENAI_API_KEY` to `.env`.
4. Run `python app/main.py`.
