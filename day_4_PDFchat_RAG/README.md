# 📚 PDF Chat Assistant using RAG

A document-based AI assistant that allows users to upload PDF files and ask questions about their content using Retrieval-Augmented Generation (RAG).

Instead of relying only on the LLM's existing knowledge, the application retrieves relevant information from uploaded documents and uses that context to generate answers.

## 🚀 Features

- Upload PDF documents.
- Extract text from PDF files.
- Split documents into smaller chunks.
- Generate and store document embeddings.
- Retrieve relevant information using ChromaDB.
- Generate context-aware answers using OpenAI.
- Interactive Streamlit interface.

## 🏗️ Architecture

1. **PDF Upload:** Users upload their PDF documents.
2. **Text Extraction:** PyPDF extracts the document content.
3. **Text Chunking:** Extracted content is divided into smaller chunks.
4. **Vector Storage:** ChromaDB stores document embeddings.
5. **Retrieval:** Relevant chunks are retrieved based on the user's question.
6. **Response Generation:** OpenAI generates an answer using the retrieved context.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core application |
| Streamlit | User interface |
| OpenAI API | LLM integration |
| ChromaDB | Vector database |
| PyPDF | PDF text extraction |
| Requests | HTTP requests |
| Python-dotenv | Environment management |

## 📁 Project Structure

```text
day_4_PDFchat_RAG/
│
├── app.py
├── llm_service.py
├── document_service.py
├── rag_service.py
├── rag_prompts.py
├── requirements.txt
├── requirements-lock.txt
├── demo_guide.md
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd day_4_PDFchat_RAG
```

### 2. Create a virtual environment

```bash
python3 -m venv .venv
```

### 3. Activate the environment

**Linux / WSL:**

```bash
source .venv/bin/activate
```

**Windows:**

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 5. Configure API credentials

Create a `.env` file in the project directory:

```env
OPENAI_API_KEY=your_openai_api_key
```

Never commit your API key to GitHub.

### 6. Run the Streamlit application

```bash
streamlit run app.py
```

Streamlit will provide a local URL, usually:

```text
http://localhost:8501
```

Open the URL in your browser to interact with the PDF Chat Assistant.

## 🧠 Understanding RAG

Retrieval-Augmented Generation combines information retrieval with generative AI.

Rather than asking an LLM to answer a question without supporting documents, RAG retrieves relevant document chunks and supplies them as context.

**Core workflow:**

PDF → Text Extraction → Chunking → Embeddings → ChromaDB → Retrieval → LLM → Answer

## 🎯 Learning Outcomes

Through this project, I explored:

- Building a document-based AI application.
- Understanding the RAG architecture.
- PDF processing and text chunking.
- Vector databases and semantic retrieval.
- Integrating LLM APIs into Python applications.
- Developing interactive AI applications using Streamlit.

---

**Project:** 7-Day Practical AI Bootcamp  
**Day:** 4  
**Focus:** Retrieval-Augmented Generation (RAG) and Document Q&A
### PDF Chat Assistant using RAG
![PDF Chat Assistant](images/pdf%20chat%20assistant%20using%20RAG.png)
### Day 4 - RAG Implementation
![RAG Implementation](images/day%204%20rag%20.png) 
