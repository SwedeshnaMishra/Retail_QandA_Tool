# Retail_QandA_Tool — AtliQ Tees: Talk to a Database

## 💬 An End-to-End LLM Project using Google PaLM & LangChain
AtliQ Tees is a T-shirt retail store that maintains its inventory, sales, and discounts data in a MySQL database.
This project builds an LLM-powered Question & Answer System that allows store managers to query the database using natural language.

---

## 🚀 Project Overview

Store managers can ask natural language questions such as:
- “How many white color Adidas t-shirts do we have left in stock?”
- “How much sales will our store generate if we sell all extra-small size t-shirts after applying discounts?”
The system intelligently:
- Converts the natural language question into an SQL query.
- Executes the query on the MySQL database.
- Returns the accurate result directly in the UI.

---

## ✨ Project Highlights

🧢 Store: AtliQ Tees sells Adidas, Nike, Van Heusen, and Levi’s T-shirts.
💾 Data: Stored in a MySQL database.

---

## 🧠 Tech Stack:

- Google PaLM LLM (via MakerSuite)
- LangChain Framework
- Hugging Face Embeddings
- ChromaDB (as Vector Store)
- Streamlit (for interactive UI)
- Few-shot Learning for prompt improvement

### 🛠️ Installation Guide: 

### 1️⃣ Clone the repository
```git clone https://github.com/codebasics/langchain.git```

### 2️⃣ Navigate to the project directory
```cd Retail_QandA_Tool```

### 3️⃣ Install dependencies
```pip install -r requirements.txt```

### 4️⃣ Set up Google API Key

- Acquire an API key from MakerSuite and create a .env file in the project root:
``` `GOOGLE_API_KEY` ="your_api_key_here"```

5️⃣ Set up the database
- Run the SQL script in your MySQL Workbench:
``` database/db_creation_atliq_t_shirts.sql```

▶️ Usage
- Run the Streamlit app:
```streamlit run main.py```
Then open the local URL (usually `http://localhost:8501`) in your browser.
You can now ask questions in natural language like:
- “How many total t-shirts are left in stock?”
- “How many Nike XS white t-shirts are available?”
- “What’s the total price of all S-size t-shirts?”
- “How much sales amount will we generate if we sell all small-size Adidas shirts after discounts?”

---

## 🧩 Project Structure
```
Retail_QandA_Tool/
│
├── main.py                 # Streamlit UI application
├── langchain_helper.py     # Core LangChain logic (LLM + SQL query generation)
├── few_shots.py            # Few-shot examples for improved accuracy
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (Google API key)
├── database/
│   └── db_creation_atliq_t_shirts.sql  # MySQL setup script
└── README.md               # Project documentation
```

---

## 💡 Example Output

- User Query:
 “How many white color Adidas t-shirts do we have left in stock?”
- System Response:
 “There are 42 white color Adidas t-shirts available in the inventory.”

---

## 📚 Future Enhancements

- Support for multiple databases (e.g., PostgreSQL, MongoDB)
- Integration with speech-to-text for voice-based queries
- Enhanced query error handling and validation
- Improved response explanation with natural language reasoning

---

## For Contributing
If you want to contribute to this project, please follow these steps:
- `Fork` the repository.
- Create a new branch `(git checkout -b feature/your-feature-name)`.
- Make your changes and commit them `(git commit -m 'Add some feature')`.
- Push to the branch `(git push origin feature/your-feature-name)`.
- Open a pull request.

---

## Project Maintainer
**Github:** [Swedeshna Mishra](https://github.com/SwedeshnaMishra)
