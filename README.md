# LangChain-Biographical-Query-Engine
This is a dual-LLM Streamlit application that showcases advanced prompt chaining, memory management, and large language model integration using OpenAI's GPT-3.5 and LLAMA2 via LangChain. The app allows users to explore biographical information about celebrities and discover historical context using multi-step sequential reasoning, and also chat dynamically with a helpful LLAMA2 assistant.

Demonstration Video: https://www.youtube.com/watch?v=xnStE21Weg4&feature=youtu.be

---

## Features

- Celebrity Exploration via OpenAI
  - Enter a name to fetch:
    - Who they are
    - Their birthdate
    - 5 major global events around their birth
- LangChain Memory
  - Stores and displays intermediate chain memory (name, date of birth, world events)
- LLAMA2-Powered Q&A Assistant
  - Uses LangChain’s prompt-template and `OllamaLLM` to answer any question via LLAMA2
-  Streamlit Frontend
  - Clean UI for query input and result expansion

---

## Tech Stack

- **LangChain**
  - `SequentialChain`, `LLMChain`, `PromptTemplate`, `ConversationBufferMemory`
- **LLMs**
  - OpenAI GPT-3.5 (via `OpenAI` integration)
  - LLAMA2 (via `OllamaLLM`)
- **Frontend**
  - Streamlit for interactive user interface
- **Environment Management**
  - `dotenv` for secure API key handling

---

##  Getting Started

1. Clone the repo

git clone https://github.com/shubham3-11/LangChain-Biographical-Query-Engine.git

cd LangChain-Biographical-Query-Engine

2. Install dependencies

pip install -r requirements.txt

3. Add your environment variables

Create a .env file in the root directory and add:

OPENAI_API_KEY=your_openai_key

LANGCHAIN_API_KEY=your_langchain_key

4. Run the app

streamlit run app.py
