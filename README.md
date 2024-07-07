PDF Query Chatbot

Introduction
The PDF Query Chatbot is a Python-based application designed to facilitate interactive conversations with multiple PDF documents. You can effortlessly inquire about the content of the PDFs using natural language, and the application will deliver pertinent responses derived from the documents. This app leverages a sophisticated language model to produce precise answers to your questions. Please note that the chatbot will only address inquiries related to the loaded PDF documents

How It Works
PDF Query Chatbot Diagram

The application follows these steps to provide responses to your questions:

PDF Loading: The app reads multiple PDF documents and extracts their text content.

Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

Dependencies and Installation
To install the PDF Query Chatbot, please follow these steps:

Clone the repository to your local machine.

Install the required dependencies by running the following command:

pip install -r requirements.txt

Obtain an API key from OpenAI and add it to the .env file in the project directory.

HUGGINGFACE_API_KEY='your_api_key_here'
Usage
To use the PDF Query Chatbot, follow these steps:

Ensure that you have installed the required dependencies and added the OpenAI API key to the .env file.

Run the main.py file using the Streamlit CLI. Execute the following command:

streamlit run app.py
The application will launch in your default web browser, displaying the user interface.

Load multiple PDF documents into the app by following the provided instructions.

Ask questions in natural language about the loaded PDFs using the chat interface.
