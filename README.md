# RAG-chatbot

# 🤖 Simple RAG Chatbot with LangChain & Gemini

## 🧠 Overview

This project presents a specialized chatbot system that merges the intelligence of a Large Language Model (LLM) with the performance of a vector search engine. Utilizing the **Retrieval-Augmented Generation (RAG)** approach, it delivers precise and context-rich answers. The interface is developed using **Streamlit**, while the backend employs **LangChain** for component integration and **Pinecone** for swift and scalable data retrieval.

---

## 🧰 Technology Stack

| Layer       | Technology         |
|-------------|--------------------|
| Frontend    | Streamlit          |
| LLM         | Gemini API         |
| Backend     | LangChain (RAG)    |
| Vector DB   | Pinecone           |
| File Parsing| PyPDF              |

---

## 📁 Project Structure

## 📁 Project Structure

| Path                    | Description                                     |
|-------------------------|-------------------------------------------------|
| `/src/`                 | Core Python files and main Streamlit app        |
| `/src/streamlitMain.py` | Entry point for launching the chatbot UI        |
| `/src/materials/`       | Domain-specific documents for context retrieval |
| `.env`                  | Environment variables (API keys)                |
| `requirements.txt`      | Python dependency list                          |
| `README.md`             | Project overview and instructions               |


🚀 Getting Started
1. Clone the Repository
bash
Copy code
git clone https://github.com/Faridghr/Simple-RAG-Chatbot.git
cd Simple-RAG-Chatbot
2. Install the Requirements
bash
Copy code
pip install -r requirements.txt
3. Set Up API Keys
Create a .env file in the root directory with the following content:

env
Copy code
GEMINI_API_KEY=your_google_gemini_api_key
PINECONE_API_KEY=your_pinecone_api_key
PINECONE_ENV=your_pinecone_environment
⚠️ Keep this file private and never upload it to version control.

💻 Running the Application
bash
Copy code
cd src
streamlit run streamlitMain.py
Then, open your browser and navigate to the URL provided (usually http://localhost:8501).

🧪 Using the Chatbot
Type your questions into the chatbot.

The system retrieves relevant context from documents using Pinecone.

Gemini API generates responses based on both the query and the retrieved content.

🔐 Setting Up Gemini API
Go to Google AI Studio

Sign in and navigate to API Keys

Generate a new API key

Copy the key and add it to your .env file as GEMINI_API_KEY

🌲 Setting Up Pinecone
Sign up at pinecone.io

Create a project (e.g., "SimpleRAGChatbot Application")

Select:

Cloud Provider: GCP

Environment: gcp-starter

Copy your API key and environment name

Add them to your .env file
