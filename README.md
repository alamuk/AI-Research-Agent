# 🧠 AI Research Assistant

This project is an AI-powered research assistant built with [LangChain](https://www.langchain.com/), [OpenAI](https://platform.openai.com/), and tool integrations for web search, Wikipedia querying, and saving output to text files.

It accepts a natural language query and returns a structured research report including a summary, sources, tools used, and optionally saves the report to a text file.

---

## 🚀 Features

- ✅ Structured research reports using Pydantic
- 🔍 Web search via DuckDuckGo
- 📚 Wikipedia lookups
- 💾 Output saving to `.txt` with timestamps
- 🧠 LLM-powered agent reasoning (via GPT-4o-mini or compatible)

---

## 🛠️ Tech Stack

- Python 3.10+
- [LangChain](https://docs.langchain.com/)
- [OpenAI GPT-4o](https://platform.openai.com/docs/models/gpt-4o)
- DuckDuckGo Search Tool
- Wikipedia Tool
- Pydantic
- dotenv for environment management

---

## 🔍 Just type in a query like - "what is the population of France in 2024 "

and get back a structured summary, verified sources, tools used, and even save the output to a local file — all handled by an intelligent agent.

## 📂 Project Structure

├── main.py # Entry point for the assistant
├── tools.py # Tool definitions (search, wiki, save)
├── .env # API keys and environment variables
├── requirements.txt # Dependencies
├── research_output.txt # (Generated) Output log file
└── README.md # You're here!

Create and activate a virtual environment:

```
python -m venv venv
source venv/bin/activate
# On Windows: venv\Scripts\activate
```

Install dependencies:

```
pip install -r requirements.txt
```

Create a .env file with your OpenAI API key:

```
OPENAI_API_KEY=your-api-key-here
```

Run the application:

```
python main.py
```

### 💡 Notes

Tool usage is intelligently managed by the agent — it avoids redundant or repeated queries.

The final response is parsed into a structured format via Pydantic.

All research outputs can be saved with the save_text_to_file tool.

### 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

### 📬 Contact

Created by MD SHAH ALAM — feel free to reach out for questions or suggestions!
