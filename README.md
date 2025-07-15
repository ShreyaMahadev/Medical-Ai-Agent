# 🏥 Medical AI Agent  
An Intelligent Symptom-Based Triage Assistant using LangGraph and Gemini

**Medical AI Agent** is a conversational AI system that simulates a hospital triage process. By taking a user’s symptom as input, it classifies the symptom using Google’s Gemini LLM and routes the case to the appropriate department: **General**, **Emergency**, or **Mental Health**. The project is built using **LangGraph**, a stateful graph-based execution framework on top of LangChain.

---

## 🚀 Features

- 🤖 Uses **Gemini (via LangChain)** for accurate symptom classification
- 🔁 Built with **LangGraph** for modular and stateful logic flow
- 🧠 Automatically routes user input to:
  - General Consultation
  - Emergency Services
  - Mental Health Support
- 💬 CLI-based interaction with human-like responses
- 🗺️ Visualizes triage logic using Mermaid flowchart

---

## 🛠️ Tech Stack

- **Python 3.11+**
- [LangGraph](https://python.langchain.com/docs/langgraph/)
- [LangChain](https://www.langchain.com/)
- [Google Generative AI](https://ai.google.dev/)
- `TypedDict` for safe, typed state management

---

## ⚙️ How It Works

1. The user is prompted to enter a symptom (e.g., "I feel anxious").
2. The symptom is sent to **Gemini** via `ChatGoogleGenerativeAI`.
3. Based on the model's response, the symptom is classified into one of three categories:
   - `General`
   - `Emergency`
   - `Mental Health`
4. **LangGraph** routes the flow to the appropriate handler node.
5. A message is returned with guidance based on the classification.

---


