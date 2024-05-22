# PDF Chatbot

## Overview

This project is an NLP chatbot that allows you to interact with multiple PDFs seamlessly. You can upload any number of PDF documents, ask questions about their content, and get natural language responses. The chatbot leverages several powerful libraries and tools to provide an intuitive and efficient user experience.

## Features

- **Multi-PDF Handling**: Upload and process multiple PDFs at once.
- **Natural Language Processing**: Ask questions in natural language and receive accurate, context-aware answers.
- **User-Friendly Interface**: Simple and interactive interface powered by Streamlit.
- **Scalable and Extensible**: Built with modular components for easy extension and scaling.

## Tech Stack

- **PyPDF2**: For handling PDF files and extracting text.
- **python-dotenv**: For managing environment variables.
- **Streamlit**: For creating the web-based user interface.
- **OpenAI**: For providing the NLP capabilities via its API.
- **LangChain**: For chaining and managing language model queries.

## Installation

### Prerequisites

- Python 3.8 or higher
- Pip (Python package installer)
- OpenAI API key

### Steps

1. **Clone the repository**:

    ```bash
    git clone https://github.com/yourusername/pdf-chatbot.git
    cd pdf-chatbot
    ```

2. **Set up a virtual environment** (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages**:

    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:

    Create a `.env` file in the project root and add your OpenAI API key:

    ```env
    OPENAI_API_KEY=your_openai_api_key
    ```

## Usage

1. **Run the Streamlit application**:

    ```bash
    streamlit run app.py
    ```

2. **Upload PDF Files**: Use the file uploader in the interface to upload the PDF documents you want to query.

3. **Ask Questions**: Enter your questions in the text input box and receive answers based on the content of the uploaded PDFs.

## Project Structure

```plaintext
pdf-chatbot/
│
├── app.py                 # Main application script
├── requirements.txt       # List of required Python packages
├── .env                   # Environment variables file (not included in repository)
├── README.md              # Project documentation
│
└── utils/                 # Utility functions and modules
    ├── pdf_handler.py     # PDF handling and text extraction
    ├── query_engine.py    # Integration with OpenAI API and LangChain
    └── interface.py       # Streamlit interface components
