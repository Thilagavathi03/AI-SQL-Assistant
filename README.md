# 👕 AI SQL Assistant – Natural Language to SQL

An AI-powered application that allows users to query a database using **natural language** and automatically converts it into **SQL queries**.

Built using **LangChain**, **Streamlit**, **MySQL**, and **Google Gemini**.

Users can ask questions like:

```
How many t-shirts are in stock?
What is the price of Nike t-shirts?
Show total sales for Adidas products
```

The system automatically:

1. Converts the question into SQL
2. Executes it on the database
3. Returns the answer to the user

---

# 🚀 Features

✅ Natural language to SQL conversion
✅ Few-shot prompting for accurate SQL generation
✅ Semantic example selection using embeddings
✅ Vector similarity search with Chroma
✅ Interactive UI with Streamlit
✅ MySQL database integration

---

# 🏗️ Project Architecture

```
User Question
      │
      ▼
Streamlit UI
      │
      ▼
LangChain SQL Chain
      │
      ▼
Gemini LLM
      │
      ▼
Generate SQL Query
      │
      ▼
MySQL Database
      │
      ▼
Return Answer to User
```

---

# 📂 Project Structure

```
AI_SQL_Assistant/
│
├── main.py
├── langchain_helper.py
├── few_shots.py
├── .env
├── requirements.txt
└── README.md
```

### main.py

Streamlit application for the user interface.

### langchain_helper.py

Creates the **LangChain SQL chain** and connects LLM + database.

### few_shots.py

Contains example question–SQL pairs used for **few-shot prompting**.

### .env

Stores API keys securely.

---

# ⚙️ Tech Stack

* Python
* LangChain
* Streamlit
* MySQL
* Google Gemini
* Chroma
* HuggingFace Embeddings

---

# 🛠️ Installation

## 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/ai-sql-assistant.git
cd ai-sql-assistant
```

---

## 2️⃣ Create virtual environment

```bash
python -m venv venv
```

Activate it

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

---

## 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

## 4️⃣ Setup Environment Variables

Create `.env`

```
GOOGLE_API_KEY=your_api_key_here
```

Get the API key from:

[https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

---

## 5️⃣ Setup MySQL Database

Create database:

```sql
CREATE DATABASE shop_tshirts;
```

Add tables and sample data.

---

## ▶️ Run the Application

```bash
streamlit run main.py
```

Open browser:

```
http://localhost:8501
```

---

# 💬 Example Queries

Try asking:

```
How many t-shirts are available in stock?

What is the price of Levi's t-shirts?

Show total inventory value
```

---

# 🧠 How It Works

1️⃣ User asks a question
2️⃣ LangChain selects relevant examples using embeddings
3️⃣ LLM generates SQL query
4️⃣ Query executes on MySQL database
5️⃣ Result returned to user

---

# 🔐 Environment Variables

```
GOOGLE_API_KEY=your_api_key
```

---

# 📸 Demo

![AI SQL Assistant Screenshot](https://raw.githubusercontent.com/Thilagavathi03/AI-SQL-Assistant/refs/heads/main/images/Screenshot%202026-03-16%20121756.png)

```
Question: How many t-shirts do we have left for Nike in XS size and white color

Answer: 38
```

---

# 📌 Future Improvements

* Add support for multiple databases
* Add query explanation feature
* Add charts for query results
* Deploy using Streamlit Cloud
* Add authentication

---


# 👩‍💻 Author

**Thilagavathi**

AI | Data | Python | SQL

---
**
