
# 📊 Gemini SQL Assistant

**Gemini SQL Assistant** is an interactive Streamlit web app that allows users to ask questions in plain English and receive SQL queries and corresponding results using Google’s Gemini 2.0 Flash model. It’s built on a sample SQLite database (`Naresh_it_employee1.db`) and is ideal for demonstrating how LLMs can simplify data exploration for non-technical users.

---

## 🚀 Features

- ✅ Natural language to SQL conversion using **Google Gemini API**  
- ✅ Support for **SQLite** queries with real-time execution  
- ✅ Automatically explains generated SQL queries in simple terms  
- ✅ Clean and user-friendly **Streamlit UI**  
- ✅ Comes with a sample dataset of employee records

---

## 📁 Project Structure

```
.
├── application.py         # Streamlit app logic and UI
├── sql.py                 # Creates the SQLite database and sample records
├── requirements.txt       # Required dependencies
└── .env                   # Stores your Gemini API key
```

---

## 🛠️ Setup Instructions

### 1. 🔑 Get Your Gemini API Key

- Go to [Google AI Studio](https://makersuite.google.com/app)  
- Create an API key under **"Get API Key"**  
- Save it in a file named `.env`:

```bash
GEMINI_API_KEY=your_api_key_here
```

### 2. 📦 Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. 🧱 Set Up the SQLite Database

```bash
python sql.py
```

This creates `Naresh_it_employee1.db` and inserts sample employee data.

### 4. ▶️ Run the App

```bash
streamlit run application.py
```

---

## 🧠 Example Questions You Can Ask

- “List all employees.”
- “Who earns more than 60,000?”
- “Count of Data Engineers?”
- “Show average salary by role.”
- “Who earns the highest salary?”

---

## 🗂️ Database Schema

**Table:** `Naresh_it_employee1`

| Column Name      | Type     |
|------------------|----------|
| employee_name    | TEXT     |
| employee_role    | TEXT     |
| employee_salary  | FLOAT    |

---

## 🙏 Acknowledgments

Special thanks to **Omkar Sir** for his invaluable guidance and mentorship throughout this project.

---

## 📌 Tech Stack

- [Streamlit](https://streamlit.io/)  
- [Google Generative AI (Gemini)](https://ai.google.dev/)  
- [SQLite3](https://www.sqlite.org/index.html)  
- [Langchain-style prompting](https://docs.langchain.com/) (inspired)
