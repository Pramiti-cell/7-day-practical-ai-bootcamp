# 📄 AI Resume Analyzer

An AI-powered resume analysis application built using Python, Streamlit and Ollama. The application analyses uploaded resumes and generates practical feedback using a Large Language Model (LLM).

## Features

- Upload resumes in PDF, DOCX or TXT format
- Paste resume text manually
- Add a job description for targeted analysis
- Generate AI-powered resume feedback
- Identify strengths, weaknesses and missing keywords
- Suggest improvements to resume content
- Download the generated analysis report

## Tech Stack

- Python
- Streamlit
- Ollama
- Llama 3.2
- PyPDF
- Python-docx
- Requests

## Application Workflow

Resume Upload → Text Extraction → Prompt Engineering → LLM Analysis → AI Feedback Report

## Project Structure

```text
Day_3_resume_analyser/
├── app.py
├── llm_service.py
├── resume_service.py
├── resume_prompts.py
├── requirements.txt
└── README.md
```

## Run Locally

1. Install the required dependencies:

```bash
pip install -r requirements.txt
```

2. Ensure Ollama is running and the Llama 3.2 model is installed.

3. Configure the `.env` file with your Ollama settings.

4. Start the application:

```bash
streamlit run app.py
```

## Learning Outcomes

- Building an AI-powered web application
- Integrating an LLM with a Python application
- Extracting text from different document formats
- Separating frontend, backend and prompt logic
- Using environment variables for configuration

*This project is an educational resume improvement tool and is not an official recruitment or hiring system.*