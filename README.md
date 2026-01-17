# 🌌 EQUINOX-AI  
### The Autonomous Financial Singularity  
**Where Quantitative Execution Meets Generative Reasoning**

Equinox-AI is not just a trading bot.  
It is a **dual-core financial operating system** that merges autonomous trading agents with a deep-research financial analyst, unified under a single **institutional-grade terminal**.

---

## 📑 Table of Contents
- [Executive Summary](#-executive-summary)
- [System Architecture](#️-system-architecture)
- [The Dual-Core Engine](#-the-dual-core-engine)
- [Technical Stack](#️-technical-stack--dependencies)
- [Installation & Setup](#-installation--setup)
- [Configuration Guide](#️-configuration-guide)
- [Risk Management Protocols](#️-risk-management-protocols)
- [Performance Metrics](#-performance-metrics)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [Disclaimer & License](#️-disclaimer--license)

---

## 🦅 Executive Summary

Modern markets suffer from **information overload but insight scarcity**.  
Equinox-AI solves this by simulating a **complete hedge fund stack in software**.

### 🔹 Key Capabilities
- **Autonomous Execution**  
  A committee of 4 AI traders (Warren, George, Ray, Cathie) debate, decide, and execute trades independently using the **Model Context Protocol (MCP)**.

- **Deep Financial Research**  
  A LangGraph-powered analyst uses **Retrieval Augmented Generation (RAG)** to answer complex questions using verified internal PDFs — not hallucinations.

- **Live Market Intelligence**  
  Integrated web scrapers analyze **Finviz & MarketWatch** sentiment to filter false signals in real time.

---

## 🏗️ System Architecture

Equinox-AI uses a **decoupled, event-driven architecture** so the Trading Engine never blocks the Research Engine.

```mermaid
graph TD
    User[User Terminal] --> UI[Gradio Unified Dashboard]

    subgraph CORE_1["CORE 1: EXECUTION ENGINE (Async Loop)"]
        UI --> TradingFloor[Trading Floor Orchestrator]
        TradingFloor --> Agents[Agent Committee]

        Agents --> Warren[Claude-3-Opus]
        Agents --> George[Gemini-Pro]
        Agents --> Cathie[GPT-4]

        Agents --> MCP[Model Context Protocol]
        MCP --> Market[Polygon.io]
        MCP --> Portfolio[SQLite Ledger]
        MCP --> Risk[VaR & Drawdown Guardrails]
    end

    subgraph CORE_2["CORE 2: INTELLIGENCE ENGINE (LangGraph)"]
        UI --> Chatbot[Analyst Chatbot]
        Chatbot --> Router[Intent Classifier]

        Router --> Sentiment[Sentiment Engine]
        Sentiment --> News[Finviz / MarketWatch]

        Router --> MF[Mutual Fund Scraper]
        Router --> RAG[RAG Pipeline]
        RAG --> VectorDB[ChromaDB]
    end

    Risk --> Alerts[Pushover Notifications]
