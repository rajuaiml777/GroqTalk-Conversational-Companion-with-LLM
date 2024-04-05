# GroqTalk-Conversational-Companion-with-LLM

![Groq Chat App](https://github.com/rajuaiml777/GroqTalk-Conversational-Companion-with-LLM/blob/main/Picture1.png)

## Overview

Groq Chat App is a simple and visually appealing web application that allows users to interact with different large language models (LLMs) using Groq and the Langchain library. With this application, users can customize the length of conversational memory, view chat history, and seamlessly communicate with language models.

## Features

- Interact with different large language models (LLMs)
- Customize the length of conversational memory
- View chat history

## Getting Started

### Dependencies

Make sure you have the following dependencies installed:

- `streamlit`
- `groq`
- `langchain`
- `langchain-groq`
- `dotenv`

### Installation

1. Create a `.env` file and include your Groq API key:

    ```
    GROQ_API_KEY=your_api_key_here
    ```

2. Run the application:

    ```bash
    streamlit run app.py
    ```

The application will open in a new browser tab.

## Usage

1. Choose a language model from the dropdown menu.
2. Adjust the conversational memory length using the slider.
3. Enter your question in the text area.
4. View the chatbot's response.
5. The chat history will be displayed below the text area.

## Code Overview

- The main function initializes the Streamlit application.
- Users can select a language model from the sidebar.
- The conversational memory length can be customized using the slider.
- User input is stored in the chat history session state.
- The `GroqChat` object initializes the Groq Langchain chat with the selected language model.
- The `ConversationChain` object initializes the conversation using the `llm` and `memory` objects.
- When the user submits a question, the application creates a new chat message and appends it to the chat history.

## License

This project is licensed under the MIT License. Feel free to customize and enhance it to meet your specific needs or preferences.

