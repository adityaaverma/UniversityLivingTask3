# End-to-end-Medical-Chatbot-using-Llama2

# How to run?
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mchatbot python=3.8 -y
```

```bash
conda activate mchatbot
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


### Create a `.env` file in the root directory and add your Pinecone credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


### Download the quantize model from the link provided in model folder & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

```bash
# run the following command
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


### Techstack Used:

- Python
- LangChain
- Flask
- Meta Llama2
- Pinecone




# Medical Chatbot using Llama-2
## Project Overview

This project involves creating a medical chatbot utilizing the Llama-2-7b-chat model in combination with Pinecone, a vector database. The chatbot fetches relevant medical information from a preprocessed medical book stored as vectors in Pinecone and delivers accurate responses based on user queries.


## Project Description

The chatbot is based on the Llama-2-7b-chat model, which interacts with a vector database created using Pinecone. The vector database is populated by converting the content of a medical book (Medical_book.pdf) into vectors. When a user interacts with the chatbot, the LLM queries the vector database to retrieve relevant information and provides accurate medical responses.

This architecture ensures that the chatbot can efficiently fetch and deliver precise medical information based on user queries, leveraging the powerful combination of Llama-2-7b-chat and Pinecone.



