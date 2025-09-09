# Cold Email Generator 📧

## Overview
The Cold Email Generator is a web-based application designed to generate personalized, AI-powered cold emails for potential clients. By scraping job details from a URL, the tool processes the data to identify job descriptions and relevant skills, matching them with AtliQ's portfolio to craft a professional email.

⚠️ **Note**: The full source code for this project is private. If you are interested in viewing the code, feel free to reach out via [yi559668@gmail.com].


---

## Screenshots

### **Main Interface**
![Main Interface](screenshots/Screenshot_(449).png)
*Caption: Enter a URL to generate a cold email.*

![Job Posting](screenshots/Screenshot_(452).png)
*Caption: Screenshot of the job posting for **Senior Software Engineer** at Nike.*


### **Generated Email**
![Generated Email](screenshots/Screenshot_(450).png)
![Generated Email](screenshots/Screenshot_(454).png)
*Caption: Example of a generated cold email.*

---

## Features
- Scrapes job postings from career websites.
- Extracts structured job details such as role, experience, skills, and description.
- Matches skills with AtliQ’s portfolio using FAISS and recommends relevant links.
- Generates AI-powered cold emails tailored to the client’s needs.

---

## Tools and Technologies
- **LangChain**: Used for creating language model chains.
- **ChatGroq (LLM)**: Llama 3.1-70b model for generating structured JSON and cold emails.
- **FAISS**: Vector search for querying AtliQ’s portfolio.
- **SentenceTransformers**: For embedding and querying skills.
- **Streamlit**: Web framework for building the user interface.
- **WebBaseLoader**: To scrape text content from URLs.
- **Pandas**: Data manipulation for handling AtliQ’s portfolio.
- **Regex (re)**: For cleaning scraped text.

---

## How It Works
1. **Input URL**:
   - The user provides a career page URL containing job postings.
2. **Scrape and Clean**:
   - The application scrapes and cleans the text from the URL using `WebBaseLoader` and `clean_text`.
3. **Extract Job Details**:
   - Using an LLM chain, the tool extracts job details in JSON format (e.g., role, skills, description).
4. **Match Portfolio**:
   - FAISS is used to query AtliQ’s portfolio, identifying the most relevant links based on required skills.
5. **Generate Cold Email**:
   - The tool uses the extracted job details and portfolio links to craft a professional cold email.

---

## Tools and File Structure
### **Key Components**
- `chains.py`:
  - Contains logic for interacting with the LLM to extract job details and generate emails.
- `main.py`:
  - Streamlit application that connects all components and provides the user interface.
- `portfolio.py`:
  - Handles AtliQ’s portfolio, creating embeddings and querying links using FAISS.
- `utils.py`:
  - Includes helper functions like `clean_text` for preprocessing scraped content.
- `.env`:
  - Stores sensitive data such as the Groq API key.

---

## Key Features
1. **Job Data Extraction**:
   - Scrapes career page content and parses it into structured JSON.
2. **Cold Email Generation**:
   - Writes professional emails tailored to each job posting.
3. **Portfolio Integration**:
   - Matches job requirements with AtliQ’s portfolio to add credibility.
4. **Interactive Web App**:
   - Built with Streamlit for a seamless user experience.



