# AskAI - Streamlit AI Assistant

This directory contains **AskAI** (AskAnish), a simple but powerful AI Assistant Chatbot built using [Streamlit](https://streamlit.io/) and [LangChain](https://www.langchain.com/), powered by the **Google Gemini 2.5 Flash Lite** model.

## Features

- **Interactive Chat Interface**: A clean, conversational UI to chat with the AI.
- **Pre-defined Suggestions**: Quick prompt buttons for common questions like latest AI trends, recipes, or quantum computing.
- **Session Memory**: The app maintains chat history within the active Streamlit session, allowing for conversational context.
- **Streaming Responses**: The assistant's replies are streamed word-by-word for a more natural, dynamic feel.

## Tech Stack

- **Frontend/UI**: [Streamlit](https://streamlit.io/)
- **LLM Orchestration**: [LangChain (`langchain-google-genai`)](https://python.langchain.com/docs/integrations/chat/google_generative_ai)
- **Generative AI Model**: Google Gemini 2.5 Flash Lite
- **Environment Management**: `python-dotenv`

## Prerequisites

Before running the application, make sure you have:
1. Python 3.8 or higher installed.
2. A valid **Google Gemini API Key**. You can obtain one from [Google AI Studio](https://aistudio.google.com/).

## Installation & Setup

1. **Navigate to the directory**:
   ```bash
   cd D:\deep-learning\dl_lab7
   ```

2. **Install the required dependencies**:
   Run the following command to install the necessary libraries:
   ```bash
   pip install streamlit langchain-google-genai python-dotenv
   ```

3. **Configure the Environment Variables**:
   Create a `.env` file in the root of the `dl_lab7` directory. Add your Google API Key to this file:
   ```env
   GOOGLE_API_KEY=your_actual_api_key_here
   ```

## Running the Application

Once your dependencies are installed and the `.env` file is set up, start the Streamlit server:

```bash
streamlit run app.py
```

The application will automatically open in your default web browser (usually at `http://localhost:8501`).

## How it Works
- The application uses `st.session_state` to store message history.
- When a user inputs a message (either via the text box or by clicking a suggestion), it is appended to the history and sent to the Gemini API via LangChain.
- The `gemini.invoke()` method receives the context and generates a response, which is then dynamically streamed onto the screen using a custom generator function.
