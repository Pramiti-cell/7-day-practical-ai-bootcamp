# Day 5 – AI Research Agent

An AI-powered research assistant built using Python, Streamlit and Ollama. The application takes a research topic, creates a research plan, retrieves relevant information from a local knowledge base, analyses the sources and generates a structured research report.

## Features

- **Research Planning:** Uses an LLM to break down a research topic into smaller research tasks.
- **Information Retrieval:** Searches a local sample knowledge base and ranks relevant sources.
- **Source Analysis:** Uses an LLM to analyse retrieved information and extract key findings.
- **Report Generation:** Produces a structured research report based on the findings.
- **Report Review:** Reviews the generated report for quality and completeness.
- **Report Export:** Allows users to download the final research report.

## Tech Stack

- Python
- Streamlit – User interface
- Ollama – Local LLM inference
- Llama 3.2 – Language model
- Requests – API communication
- Python-dotenv – Environment variable management

## How It Works

1. The user enters a research topic.
2. The AI creates a research plan.
3. The search tool retrieves relevant information from a local knowledge base.
4. The LLM analyses the retrieved sources.
5. The agent generates a structured research report.
6. The report is reviewed and made available for download.

## Project Structure

```text
day_5_research_agent/
│
├── app.py
├── research_agent.py
├── search_tool.py
├── llm_service.py
├── agent_prompts.py
├── .env.example
├── requirements.txt
└── README.md
```

## Setup and Installation

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd day_5_research_agent
```

### 2. Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create your `.env` file using the example:

```bash
cp .env.example .env
```

Configure your Ollama connection:

```env
LLM_PROVIDER=ollama
OLLAMA_MODEL=llama3.2:1b
OLLAMA_URL=http://YOUR_OLLAMA_HOST:11434/api/chat
```

Do not commit your `.env` file or API keys to GitHub.

### 5. Start Ollama

Make sure Ollama is running and the selected model is available.

```bash
ollama pull llama3.2:1b
```

### 6. Run the application

```bash
streamlit run app.py
```

## Example Research Topic

"How can small businesses use AI to improve customer support?"

The agent uses the topic to create a research plan, retrieve relevant sources, analyse findings and generate a final report.

## What I Learned

- Building a multi-step AI agent workflow.
- Connecting Python applications to locally hosted LLMs.
- Sending API requests to Ollama.
- Designing prompts for planning, analysis and report generation.
- Implementing keyword-based information retrieval.
- Organising an AI project using modular Python files.
- Integrating an AI backend with a Streamlit interface.

## Future Improvements

- Integrate live web search for external research.
- Add vector-based semantic search.
- Support multiple research topics and source formats.
- Improve source relevance and report evaluation.
- Add citation generation and source verification.
![AI Research Agent](images/day%205%20autonomous%20research%20agent.png)
![Slide 2](images/day%205%20slide%202.png)
![Slide 3](images/day%205%20slide%203.png)