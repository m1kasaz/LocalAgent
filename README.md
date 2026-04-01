# LocalAgent

![LangChain](https://img.shields.io/badge/Framework-LangChain-blue.svg)
![Python](https://img.shields.io/badge/Python-3.9+-green.svg)
![License](https://img.shields.io/badge/License-MIT-orange.svg)

`LocalAgent` 是一个基于 **LangChain** 构建的智能化 Agent 框架。它通过集成 **向量数据库** 实现增强检索（RAG），并利用 **持久化存储** 机制赋予智能体长短期记忆能力，旨在打造一个可本地部署、高扩展性的私人知识库助手。

---

## 🚀 核心特性

- **向量检索增强 (RAG)**：支持 PDF、Markdown、Docx 等多种格式文档的自动化清洗、切片及向量化存储。
- **多维记忆管理**：
    - **短期记忆**：基于对话上下文的 Window Buffer，确保对话连贯。
    - **长期记忆**：支持将历史对话持久化至数据库（如 SQLite/Redis），实现跨会话记忆。
- **动态工具链 (ReAct)**：智能体可根据用户需求自动调用外部工具（如搜索、计算器、API 请求）。
- **灵活的后端适配**：完美支持 OpenAI、Anthropic 等在线模型，以及通过 **Ollama** 接入的本地模型（Llama 3, Qwen 2 等）。

## 🛠️ 技术栈

* **核心框架**: [LangChain](https://github.com/langchain-ai/langchain)
* **向量数据库**: ChromaDB / FAISS
* **嵌入模型 (Embeddings)**: OpenAI / HuggingFace (Sentence-Transformers)
* **大语言模型**: GPT-4o / Llama 3 (Local)
* **存储层**: SQLite / PostgreSQL

