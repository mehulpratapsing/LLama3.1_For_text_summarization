# LLama3.1_For_text_summarization
Google Colab notebook for utilizing Llama 3.1 for text summarization

# Text Extraction and Summarization with Ollama

This repository provides a Python script to extract text from various file formats (PDF, DOCX, DOC, and TXT) and then summarize the extracted text using the Ollama model. The script is designed to be run in a Google Colab environment.

## Requirements

Make sure you have the following libraries installed in your Colab environment:

- `colab-xterm`
- `langchain_community`
- `fitz` (PyMuPDF)
- `python-docx`
- `pypandoc`
- `pandoc`

## Installation

First, install the required packages and set up the terminal environment:

```python
!pip install colab-xterm langchain_community fitz python-docx pypandoc
!apt-get install pandoc
%load_ext colabxterm

###################################

%xterm
# Inside the terminal
curl -fsSL https://ollama.com/install.sh | sh
ollama serve & ollama pull llama3.1
