# News Research Tool 📈

This repository contains a Streamlit application for researching news articles. The application allows users to input URLs of news articles, process the text content, and perform searches on the processed data using OpenAI's language model. The application utilizes various components from the LangChain library to load, split, embed, and retrieve information from the articles.

## Features

- **Streamlit Interface**: User-friendly interface for inputting URLs and searching content.
- **Data Loading**: Load and process text content from the provided URLs.
- **Text Splitting**: Split the text content into manageable chunks for processing.
- **Embeddings**: Generate embeddings using OpenAI's language model.
- **Vector Store**: Store and retrieve document embeddings using FAISS.
- **Search Functionality**: Perform searches on the processed data and get answers with sources.

## Setup

### Prerequisites

- Python 3.8+
- Streamlit
- OpenAI API key

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/esha1231/News-Research-Tool.git
    cd News-Research-Tool
    ```

3. Install the required packages:
    ```sh
    pip install langchain
    pip install -U langchain-community
    pip install unstructured python-magic libmagic
    pip install faiss-cpu
    pip install python-dotenv
    pip install streamlit
    pip install tiktoken
    ```

4. Create a `.env` file in the root directory and add your OpenAI API key:
    ```env
    OPENAI_API_KEY=your_openai_api_key
    ```

## Usage

1. Run the Streamlit application:
    ```sh
    streamlit run main.py
    ```

2. Open your browser and go to `http://localhost:8501`.

3. In the sidebar, input up to three URLs of news articles you want to process.

4. Click the "Process URLs" button to start processing.

5. Once processing is complete, input your search query in the main interface and press Enter.

6. View the search results and the sources of the information.
