# Chat-with-PDFs

## Intro

The PDF Chat App is a Python application that allows you to chat with multiple PDF documents. You can ask questions about the PDFs using natural language, and the application will provide relevant responses based on the content of the documents. This app utilizes a language model to generate accurate answers to your queries. Please note that the app will only respond to questions related to the loaded PDFs.

## How It Works

The application follows these steps to provide responses to your questions:

1. PDF Loading: The app reads multiple PDF documents and extracts their text content.

2. Text Chunking: The extracted text is divided into smaller chunks that can be processed effectively.

3. Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

   ![PDF-LangChain](https://github.com/Alwyn25/Chat-with-PDFs/assets/99828232/c3803d8c-90c8-4327-aaba-a5a2ffac0e4b)

## Dependencies and Installation

To install the MultiPDF Chat App, please follow these steps:

Clone the repository to your local machine.

Install the required dependencies by running the following command:

  pip install -r requirements.txt
  
Obtain an API key from OpenAI and add it to the .env file in the project directory.

  OPENAI_API_KEY=your_secrit_api_key

## Usage

To use the MultiPDF Chat App, follow these steps:
1. Ensure that you have installed the required dependencies and added the OpenAI API key to the .env file.
2. Run the main.py file using the Streamlit CLI. Execute the following command:
     streamlit run app.py
4. The application will launch in your default web browser, displaying the user interface.
5. Load multiple PDF documents into the app by following the provided instructions.
6. Ask questions in natural language about the loaded PDFs using the chat interface.
