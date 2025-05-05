# MedWise - Knowledge-Based Medical Chatbot

MedWise is an intelligent, RAG-based (Retrieval Augmented Generation) chatbot designed to answer medical queries using information extracted from **The GALE Encyclopedia of Medicine (2nd Edition)**. It integrates **Pinecone** for vector storage, **Gemini 2.0 Flash LLM** for response generation (via API), and a **Flask** web app for the frontend interface.

---

## Features

- Knowledge-based retrieval from a trusted medical source  
- Intelligent and context-aware chatbot responses using Gemini 2.0 Flash  
- Fast semantic search with Pinecone vector database  
- RAG Architecture: Combines retrieval with generation for accurate, up-to-date answers  
- Flask-based user interface  

---

## 🛠️ Tech Stack

- **Python**
- **LangChain**
- **Flask**
- **Pinecone Vector DB**
- **Gemini 2.0 Flash (via API)**
- **RAG (Retrieval Augmented Generation) Architecture**
# How to run?
### STEPS:

clone the repositroy

``` bash
project repo: https://github.com/
```
### STEP 01-create a conda enviroment after opening the repo

``` bash
conda create -n medwise python=3.10 -y
```
```bash
conda activate medwise
```

### STEP 02-install the requirments

```bash 
pip install -r requirements.txt
```
### Create a `.env` file in the root directory and add your Pinecone & openai credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
OPENAI_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


```bash
# run the following command to store embeddings to pinecone
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```

