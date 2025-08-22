
<img width="1900" height="775" alt="Screenshot 2025-08-22 234356" src="https://github.com/user-attachments/assets/671b5da5-a761-4994-b5ec-35b95b0b0ec8" />



* `langchain_helper.py`
* `few_shot.py`
* `main.py`
* `requirements.txt`

Here’s a simple version:

---

# Retail Query Assistant

This project is an AI-powered Retail Query Assistant for a fictional T-shirt store that sells Adidas, Nike, Van Heusen, and Levi's T-shirts.
The system allows users to ask natural language questions about inventory, sales, and discounts.
It then converts these questions into SQL queries using LangChain and Google Gemini, retrieves results from a MySQL database, and returns structured answers.
## Project Structure

```
Retail-Query-Assistant/
│── main.py              # Entry point for running the assistant
│── langchain_helper.py  # Functions for interacting with LangChain & Gemini
│── few_shot.py          # Few-shot examples to guide query generation
│── requirements.txt     # Dependencies
│── README.md            # Project documentation


## Features

* Converts natural language queries into SQL queries
* Uses LangChain with Gemini for LLM-based query generation
* Few-shot learning examples for improving model accuracy
* Connects to a MySQL retail database
* Provides insights such as stock status, sales queries, and more

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/adinath09/retail-query-assistant.git
   cd retail-query-assistant
   ```

2. Create a virtual environment and install dependencies:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Set up environment variables for your Gemini API key and database credentials:

   ```bash
   export GEMINI_API_KEY=your_api_key
   export DB_HOST=localhost
   export DB_USER=username
   export DB_PASS=password
   export DB_NAME=retail_db
   ```

## Usage

Run the main script:

```bash
streamlit run main.py
```

Then enter your queries in plain English, for example:

```
How many T-shirts are in stock?
Show me sales of red T-shirts last month.
```

The assistant will translate these into SQL and fetch results from the database.

## Requirements

All dependencies are listed in `requirements.txt`.

Install them with:

```bash
pip install -r requirements.txt
```

---


