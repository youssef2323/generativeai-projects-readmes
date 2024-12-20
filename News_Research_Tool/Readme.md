# News Research Tool 📈

## Overview
The News Research Tool is an AI-powered application that allows users to extract, process, and analyze content from news articles. By entering article URLs, the tool processes the text, generates embeddings, and provides answers to user queries with references to the original articles.

⚠️ **Note**: The full source code for this project is private. If you are interested in viewing the code, feel free to reach out via [yi559668@gmail.com].


---

## Screenshots

### **Main Interface**
![Main Interface](screenshots/Screenshot_(447).png)
*Caption: Enter up to three news article URLs for processing.*

### **Example Input: URLs**
![Example URLs](screenshots/Screenshot_(433).png)
![Example URLs](screenshots/Screenshot_(434).png)
![Example URLs](screenshots/Screenshot_(448).png)
*Caption: Sample URLs entered for processing.*

### **Processing URLs**
![Processing URLs](screenshots/Screenshot_(436).png)
*Caption: Tool processing the provided URLs and building embeddings.*

### **Query Result**
![Query Result](screenshots/Screenshot_(435).png)
![Query Result](screenshots/Screenshot_(437).png)
![Query Result](screenshots/Screenshot_(439).png)
![Query Result](screenshots/Screenshot_(440).png)
![Query Result](screenshots/Screenshot_(442).png)
![Query Result](screenshots/Screenshot_(443).png)
![Query Result](screenshots/Screenshot_(445).png)
*Caption: Example query and the corresponding answer with sources.*

---

## Features
- Extracts content from up to three news article URLs.
- Splits and processes text into manageable chunks for analysis.
- Utilizes FAISS for efficient vector-based retrieval of relevant information.
- Allows users to ask questions about the content and retrieves answers along with sources.
- Interactive web-based interface powered by Streamlit.

---

## Tools and Technologies
- **LangChain**: Framework for integrating language models into applications.
- **OpenAI GPT-4**: Used for text embeddings and question-answering.
- **FAISS**: Efficient vector-based retrieval for semantic search.
- **Streamlit**: Provides a user-friendly web interface.
- **dotenv**: Manages API keys securely.
- **UnstructuredURLLoader**: Extracts raw text from the provided URLs.

---

## How It Works
1. **Input URLs**: Users enter up to three news article URLs into the sidebar.
2. **Process URLs**:
   - The tool loads data from the URLs using `UnstructuredURLLoader`.
   - Text is split into manageable chunks using `RecursiveCharacterTextSplitter`.
   - Embeddings are created using OpenAI embeddings, and the data is stored in a FAISS index.
3. **Query and Retrieval**:
   - Users input a question in the main interface.
   - The FAISS index is queried to find the most relevant chunks of text.
   - Answers and sources are generated using OpenAI's language model and retrieval chain.
4. **Display Results**:
   - The tool displays the answer to the question.
   - References to the original articles are provided for transparency.

---

## Key Features
- **Embeddings with FAISS**: Converts text into semantic vectors for efficient similarity search.
- **Dynamic Content Processing**: Automatically loads and splits article content for analysis.
- **AI-Powered Q&A**: Generates answers and identifies relevant sources using OpenAI and LangChain.
- **Interactive Design**: Easy-to-use Streamlit interface for entering URLs and questions.

---

## Future Enhancements
- Support for additional URL formats and content types.
- Enhanced question-answering accuracy with fine-tuned language models.
- Improved UI/UX for better interactivity and feedback.


