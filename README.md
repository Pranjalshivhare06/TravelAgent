# ✈️ AI Travel Booking System

An AI-powered multi-agent travel planner built using **LangGraph, Groq LLM, and Streamlit**. It coordinates specialized AI agents to search for flights and hotels, generate personalized itineraries, and deliver a consolidated travel plan.

## 🚀 Features

- **Flight Agent:** Fetches flight information using AviationStack API.
- **Hotel Agent:** Searches for hotel recommendations using Tavily.
- **Itinerary Agent:** Generates travel itineraries using Groq LLM.
- **Final Agent:** Combines all results into a complete travel plan.
- **Persistent Memory:** Uses PostgreSQL checkpointing to maintain conversation state.
- **Interactive UI:** Streamlit frontend with live agent execution and downloadable travel plans.

## 🛠️ Tech Stack

- Python
- LangGraph & LangChain
- Groq LLM (`openai/gpt-oss-20b`)
- Streamlit
- PostgreSQL
- Tavily Search API
- AviationStack API

## ⚙️ Setup & Installation

**1. Clone the repository**

```bash
git clone https://github.com/Pranjalshivhare06/TravelAgent.git
cd TravelAgent
```

**2. Create and activate virtual environment**

```bash
python -m venv venv
venv\Scripts\activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Configure environment variables**

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
TAVILY_API_KEY=your_tavily_api_key
AVIATIONSTACK_API_KEY=your_aviationstack_api_key
DATABASE_URL=your_postgresql_connection_string
```

**5. Run the application**

```bash
streamlit run frontend.py
```

## 🔄 Agent Workflow

```text
User Query
    ↓
Flight Agent
    ↓
Hotel Agent
    ↓
Itinerary Agent
    ↓
Final Agent
    ↓
Complete Travel Plan
```
