
# Text Summarizer using LLM



## Table of content

  1.	Objective
  2.	Definitions
  3.	Creating virtual environment
  4. Setup


## Objective

The objective of the project is to develop a text summarization system leveraging Large Language Models (LLMs) to automatically generate concise and informative summaries of given texts. The system aims to accurately capture the key points and essential information from the input text, while ensuring coherence and readability in the generated summaries.

## Definitions

  #### CTransformers

  - Transformer is a python binding for Transformer models implemented in C/C++ using GGML library. This library provides similar interface as the Hugging Face transformer library.
  -	Used to load LLM models.
  - **GGML** : GGML is a tensor library for machine learning which enables the faster execution of large models such as LLMs on regular hardware. 

  #### Streamlit
  - It is a python framework used for creating a UI.
  - **streamlit_chat** : It provides a chat like UI.

  #### CharacterTextSplitter

  - CharacterTextSplitter extends TextSplitter and splits text into chunks based on a character, such as a newline character
  - It have mainly two parameters i.e **chunk_size** and **chunk_overlap**

## Creating virtual environment
  For creating a virtual environment follow the below steps
- **Step 1**

      Open command prompt from the search bar or press ( windows + R ) and write cmd hit enter.
	
- **Step 2**
  
  Move to the folder where you want to create the virtual environment and run the below command

      python -m venv langchain

  where, langchain is the environment name.

- **Step 3**

  Write activate and hit enter it will activate your environment

      activate



## Setup

**Step 1**

Clone the github repo

    git clone https://github.com/Sankalp-Pattanayak/Text-Summarizer.git

**Step 2**

Create and activate your virtual environment as show above.

Install the necessary packages

    pip install -r requirements.txt

**Step 3**

Now download the model file using the below link

[Download LLM Model](https://www.dropbox.com/scl/fi/080hss9a1xztrv6y0fxls/llama-2-7b-chat.ggmlv3.q2_K.bin?rlkey=xgpoctoro7ensk5fei09et6ws&dl=0)

**Step 4**

Run the application

    streamlit run app.py
