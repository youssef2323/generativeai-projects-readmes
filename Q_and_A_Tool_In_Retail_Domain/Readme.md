# Atliq T-Shirts Database Q&A

## Overview
Atliq T-Shirts Database Q&A is a web-based application that allows users to ask natural language questions about a t-shirt inventory database. The application uses AI-powered tools to dynamically generate SQL queries, fetch data from the database, and provide accurate, real-time answers.

---

## Screenshots

### **Main Interface**
![Main Interface](screenshots/Screenshot_(415).png)
*Caption: Streamlit app interface.*

### **Example Output**
![Example Output](screenshots/Screenshot_(423).png)
![Example Output](screenshots/Screenshot_(424).png)
![Example Output](screenshots/Screenshot_(425).png)
![Example Output](screenshots/Screenshot_(426).png)
![Example Output](screenshots/Screenshot_(428).png)
![Example Output](screenshots/Screenshot_(429).png)
![Example Output](screenshots/Screenshot_(431).png)
![Example Output](screenshots/Screenshot_(432).png)
*Caption: Generated SQL query and answer.*

---

## Features
- Interactive Q&A interface for database queries.
- AI-powered SQL query generation using natural language input.
- Semantic similarity matching for improved query accuracy.
- Supports inventory, pricing, and discount-related questions.

---

## Tools and Technologies
- **LangChain**: Framework for connecting language models to databases.
- **OpenAI GPT-4**: Language model for SQL generation and answer formulation.
- **HuggingFace Embeddings**: For semantic similarity-based example selection.
- **FAISS**: Vector search library for storing and retrieving few-shot examples.
- **MySQL**: Database for inventory and pricing data.
- **Streamlit**: Web framework for building the user interface.
- **dotenv**: Securely manages API keys and credentials.

---

## How It Works
1. User enters a natural language question (e.g., "How many Levi's shirts are in stock?").
2. The system retrieves the most relevant few-shot examples using FAISS and semantic similarity.
3. LangChain generates a SQL query tailored to the user’s question.
4. The query is executed on the MySQL database to fetch results.
5. The result is processed into a natural language answer and displayed in the app.

---

## Key Features
- **Few-Shot Learning**: Predefined examples guide SQL query generation.
- **Semantic Similarity Matching**: Ensures accurate example selection.
- **Dynamic Query Execution**: Interprets user questions to generate and execute SQL queries.
