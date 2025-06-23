# AzureAgenticLab

This is a modular Agentic AI application built using **Python** and **Streamlit**, powered by **Azure OpenAI**. The agent intelligently selects from multiple tools to fulfill user queries — including RAG-based search, text summarization, and domain-specific logic.

## Features

✅ Tool-usage based LLM agent (function router)  
✅ Integrates with **Azure OpenAI GPT-4o**  
✅ Built-in **Streamlit** UI  
✅ Supports 4 Tools:
- `calculate_bmi(weight, height)` – for health-related queries
- `get_financial_advice(income, expenses)` – for finance questions
- `summarize_text(text)` – for summarization tasks
- `call_rag_chat_api(query)` – for internal IT, Azure, or policy-based queries

## Folder Structure

agentic_ai/
├── app/
│   ├── agent_chat.py              # Main agent routing logic
│   ├── config.py                  # Azure OpenAI & App settings
│   ├── openai_client.py           # AzureOpenAI client setup
│   └── tools/
│       ├── calculate_bmi.py       # Tool 1 - BMI calculator
│       ├── get_financial_advice.py# Tool 2 - Financial advice
│       ├── summarize_text.py      # Tool 3 - Text summarizer
│       └── rag_call.py            # Tool 4 - Calls RAG Chat API (.NET)
│
├── webapp/
│   └── streamlit_app.py           # Streamlit UI entry point
├── .env                           # Local environment variables
├── requirements.txt
└── README.md

