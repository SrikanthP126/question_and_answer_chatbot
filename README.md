# Enhanced Q&A Chatbot with Open Source Language Models

This project is a straightforward chatbot that answers your questions smartly using open-source language models. It’s designed to be practical, easy to use, and visually interactive. The application uses LangChain for managing prompts, Ollama API for working with the language models, and Streamlit to give you a simple yet functional web interface.

## Why This Project is Cool

- **Open Source Models**: It works with models like Mistral. More options can be added in the future.
- **Customizable Responses**: You can adjust how creative or detailed the chatbot is by changing sliders for temperature and token limits.
- **Easy Monitoring**: Includes LangSmith tracking to see what the chatbot is up to behind the scenes.
- **Secure Setup**: Sensitive information like API keys is managed safely using `.env` files.
- **Super Simple UI**: Just open the app, ask your question, and get answers instantly!

## How to Set It Up

Follow these steps to get the chatbot running on your computer:

### What You’ll Need
- Python 3.8 or later
- An OpenAI account and API key for LangSmith
- A `.env` file to securely store your API key

### Steps to Install and Run

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/SrikanthP126/question_and_answer_chatbot.git  
    ```

2. **Install Required Libraries**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Set Up API Key**:
    Create a `.env` file in the root folder and add:
    ```env
    LANGCHAIN_API_KEY=your-api-key
    ```

4. **Run the App**:
    ```bash
    streamlit run app.py
    ```

5. Open your browser and go to `http://localhost:8501`.

## How to Use the Chatbot

1. From the sidebar, pick a model like Mistral (more models can be added later).  
2. Use the sliders to adjust how the chatbot responds (e.g., creativity and wordiness).  
3. Type your question into the input box and press Enter.  
4. The chatbot will reply instantly on the screen!

## Tools and Technologies

- **Python**: Backend for the chatbot logic.
- **Streamlit**: For the web app interface.
- **LangChain**: To manage and structure chatbot conversations.
- **Ollama API**: To interact with powerful open-source language models.
- **dotenv**: For secure handling of environment variables.

## Folder Structure

```plaintext
.
├── app.py             # Main Python script for the Streamlit app
├── requirements.txt   # List of libraries needed for the project
├── .env               # File to store API keys securely (not shared in the repo)
└── README.md          # This document
