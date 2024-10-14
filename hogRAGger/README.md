# Hogragger

Hogragger is an open-source hybrid search engine combining FAISS-based dense retrieval and BM25-based lexical search for document retrieval. It also includes a question-answering component powered by Hugging Face models.

### File Structure is as Follows:
this Folder contains <br>
* two data set files: -corpus.json<br>
                     -train.json
* hogRAGger.ipynb - this file is colab notebook of the full RAG pipeline you can go through it and see the full RAG implimentation
* hogRAgger_app.ipynb - this file is webapp file of colab with RAG pipeline you can also see that for webapp References (Web app is build on streamlit in colob only to run model efficiently)       

## Features

- Hybrid search combining dense embeddings (FAISS) and BM25 (lexical search)
- Automated question type classification using transformer models
- Question-answering system using pre-trained transformer models
- Retrieval of relevant passages and extraction of facts

## Requirements

- Python 3.8+
- Hugging Face `transformers`
- FAISS
- `sentence-transformers`
- `nltk`
- `rank-bm25`
-streamlit

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/hogragger.git
    cd hogragger
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Download NLTK data (optional, but needed for sentence tokenization):
    ```python
    import nltk
    nltk.download('punkt')
    ```

4. Add your `corpus.json` file in the root directory.

## Usage
you can run this on streamlit:
Installation
Step 1: Install Required Libraries
First, install the necessary libraries by running the following command:

bash
Copy code
pip install -r requirements.txt
Step 2: Download the Code
To download the code, use the following command:

bash
Copy code
!wget -q -O - ipv4.icanhazip.com
Step 3: Save the Code
Create a Python file named app.py and write the code from the repository into this file.

Step 4: Run the Application
Run the Streamlit application and expose it to the internet using LocalTunnel with the following command:

bash
Copy code
!streamlit run app.py & npx localtunnel --port 8501
Step 5: Access the Application
Once the application is running, you will receive a public URL. Click on this URL to access the application.

Step 6: Query the Application
In the provided text box, enter your query and submit it. The application will process your query and return relevant information.

Important
Upload the Corpus Dataset: Don’t forget to upload the corpus dataset (corpus.json) to the appropriate directory before running the application.