# Restaurant Name Generator

## Overview
Restaurant Name Generator is a web-based application that allows users to generate creative restaurant names and corresponding menu items based on a selected cuisine type. The application uses AI-powered tools to provide meaningful outputs tailored to user preferences.

---

## Screenshots

### **Main Interface**
![Main Interface](screenshots/Screenshot_(412).png)
*Caption: Streamlit app interface for selecting cuisine type.*

### **Example Output**
![Example Output](screenshots/Screenshot_(410).png)
![Example Output](screenshots/Screenshot_(411).png)
![Example Output](screenshots/Screenshot_(413).png)
![Example Output](screenshots/Screenshot_(414).png)
*Caption: Generated restaurant name and menu items.*

---

## Features
- Generate unique restaurant names based on a selected cuisine (e.g., Indian, Italian, Mexican, etc.).
- Provide a list of menu items customized to the restaurant theme.
- Interactive user interface for exploring various cuisines.

---

## Tools and Technologies
- **LangChain**: Framework for integrating language models into the application.
- **OpenAI GPT-4**: Language model for generating restaurant names and menu items.
- **Streamlit**: Web framework for creating a user-friendly interface.
- **dotenv**: Manages API keys and credentials securely.

---

## How It Works
1. User selects a cuisine type from the interactive sidebar (e.g., Indian, Italian).
2. The application uses pre-defined prompts to generate a restaurant name and menu items.
3. LangChain processes the prompts and retrieves results via the OpenAI API.
4. The generated restaurant name and menu items are displayed in the app interface.

---

## Key Features
- **AI-Powered Generation**: Creates restaurant names and themed menus dynamically.
- **Interactive Design**: Users can select cuisines and instantly see the results.
- **Streamlined Prompts**: Designed for seamless integration with OpenAI's GPT models.

---

## Future Enhancements
- Add support for more cuisines and menu customization options.
- Include visual elements (e.g., logos or dish images) to enhance user experience.
- Improve performance with caching for frequently requested cuisines.
