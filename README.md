## Project Overview
This is an end-to-end Large Language Model (LLM) project designed for AtliQ Tees, a T-shirt store, to manage inventory and sales data using natural language queries. Store managers can ask questions in plain English, and the system interprets these questions, converting them into SQL queries to retrieve relevant information from a MySQL database.

### Examples:

- “How many white Adidas T-shirts are left in stock?”
- “What will our sales be if we sell all extra-small T-shirts at the discounted price?”
- The project leverages Hugging Face’s API for language understanding, Langchain for query handling, and various other tools to build a robust, interactive query system.

### Project Highlights
- Store Overview: AtliQ Tees offers a range of T-shirt brands, including Adidas, Nike, Van Heusen, and Levi's.
- Data Storage: Inventory, sales, and discount data are stored in a MySQL database.
### System Components:
- Hugging Face API: Provides natural language understanding for converting user questions into SQL queries.
- Streamlit: Creates an intuitive interface for store managers.
- Langchain: Facilitates LLM integration and manages question-to-query transformations.
- ChromaDB: Acts as a vector store to improve context and query relevance.
- Few-shot Learning: Enables the system to handle diverse question types accurately.
With this setup, store managers can ask questions in everyday language, and the system produces accurate responses using the MySQL database.


## Installation

1. Clone this repository to your local machine:
   
```bash
git clone https://github.com/your-repo.git
```
2. Navigate to the project directory:
   
```bash
cd your-directory
```

3. Install required dependencies:
   
```bash
pip install -r requirements.txt
```
4. Set up Hugging Face API key:
```
HUGGINGFACE_API_KEY="your_api_key_here"
```

5. Database Setup:

 Run the database/db_creation_atliq_t_shirts.sql script in MySQL Workbench to create and initialize the necessary tables and data.

# Usage
Run the Streamlit application:

```bash
streamlit run main.py
```

### Ask Questions:

- Use the Streamlit interface to ask questions like:
- “How much revenue will we generate if all T-shirts sell out?”
- “What are the stock levels for Nike brand T-shirts?”
  
### Get Answers:

The system interprets the question, converts it into an SQL query, executes it in MySQL, and returns an answer based on AtliQ Tees’ data.
