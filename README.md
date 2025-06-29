````markdown
# 📨 Personalized Email System

An automated tool to find real estate companies, extract CEO contact details, and generate personalized outreach emails using LLMs.

---

## 🔧 What It Does

1. **Searches the Web** for real estate company leadership pages (via Tavily).
2. **Extracts URLs** from search results.
3. **Scrapes Contact Info** like CEO name, email, phone, and company (via Firecrawl).
4. **Stores Data** in Airtable.
5. **Generates Personalized Emails** using OpenAI and LangChain.

---

## ⚙️ Setup

1. **Clone the repo**
```bash
git clone https://github.com/your-username/personalized-email-system.git
cd personalized-email-system
````

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Add your API keys**
   Copy `.env.example` to `.env` and fill in:

```env
OPENAI_API_KEY=
FIRECRAWL_API_KEY=
AIRTABLE_API_KEY=
```

---

## ▶️ Run the Workflow

```python
from personalized_email import graph
result = graph.invoke({})
```

To view the generated emails:

```python
from IPython.display import Markdown
Markdown(result["email_drafts_markdown"])
```

---

## 📌 Notes

* Only a subset of results are stored in Airtable.
* Emails are tailored to CEOs with available email addresses.
* Designed for real estate but adaptable for other domains.

---

## 📄 License

MIT License

```

---

This version gives users everything they need—**what it does, how to run it, and what tools it uses—clearly and briefly**. Let me know if you want to add usage examples or visuals.
```
