# 🦙 LlamaPDFBot - LLAMA 3.1

This is a **Streamlit-based PDF chatbot** that enables users to upload a **PDF document** and interact with it using **LLAMA 3.1-70B** via **Groq**. It uses **FAISS vector storage** and **Hugging Face embeddings** for efficient document retrieval and chat memory.

## Key Highlights:
✅ Developed an AI-powered chatbot using LLAMA 3.1-70B via Groq for document-based question-answering.
✅ Built a PDF processing pipeline that extracts, splits, and embeds text using Hugging Face embeddings and stores it in FAISS for efficient retrieval.
✅ Designed and implemented a Retrieval-Augmented Generation (RAG) system, ensuring accurate and context-aware responses.
✅ Integrated Streamlit for an interactive UI, enabling users to upload PDFs, ask questions, and receive responses dynamically.
✅ Implemented Conversational Memory using LangChain’s ConversationBufferMemory, maintaining chat history for a seamless experience.
✅ Utilized LangChain for efficient document chunking, embedding creation, and retrieval optimization.
✅ Optimized model performance by fine-tuning retrieval settings and reducing response latency using efficient text-splitting strategies.
✅ Implemented secure API handling using .env files to manage Groq API keys and ensure data protection.
✅ Followed Agile development methodologies for iterative improvements and deployed locally with Python virtual environments for dependency management.

## Features
- 📄 **PDF Upload & Processing**: Extracts text from uploaded PDFs.
- 🧠 **Vector Embeddings**: Uses **FAISS** and **Hugging Face** for document storage.
- 🤖 **Conversational AI**: Implements **LLAMA 3.1-70B** via **Groq**.
- 🔍 **Retrieval-Augmented Generation (RAG)**: Provides responses based on document content.
- 💬 **Chat Memory**: Stores conversation history.

## Installation
### 1️⃣ Clone the Repository
git clone https://github.com/ratnesh134/LlamaPDFBot.git
cd chat-with-doc-llama

### Setting up the Virtual Environment
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate  # Windows

### Installing the dependencies
pip install -r requirements.txt

### Set Up API Keys
Create a .env file in the project root and add your API keys:

GROQ_API_KEY=your_groq_api_key

### Run the Application
streamlit run app.py

## Usage

Upload a PDF document.

Ask questions related to the document.

The chatbot retrieves relevant content and provides context-aware responses.

Conversation history is maintained for continuity.

## Technologies Used
Streamlit for UI

LangChain for LLM interactions

FAISS for vector search

Hugging Face Embeddings for document representation

Groq for LLAMA 3.1-70B

# Here's a flow diagram representing the workflow of your Chat with Doc - LLAMA 3.1 project.

## Flow Breakdown:
User Uploads PDF → The PDF document is loaded and processed.

Text Extraction & Splitting → The document is converted into text chunks.

Vector Embedding → Text chunks are embedded using Hugging Face Embeddings and stored in FAISS.

User Asks a Question → The query is processed and retrieved from the vector store.

LLAMA 3.1 Model Processing → The Groq LLM answers based on retrieved content.

Response Displayed → The answer and relevant document context are shown in Streamlit.
