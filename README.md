# rag-agent
RAG (Retrieval Augmented Generation) agent for students to consult with him on olympiads and solving various tasks from math and physics

## background
This model was created for the comptition between students of "Neural Network Course" in Letovo School. We were provided with various education documents and asked to create a RAG agent that will answer the questions based on the provided information

## preprocessing
To avoid suffering with different encodings of .pdf and .docx files I turned them into txt files with services which you may easily find on the internet. I also used Deepseek to extract the data structured in tables inside pdf files.

## deploying the model
With desire to create stable and efficient RAG agent I decided to use opensourse models from HuggingFace (in my case, 'BAAI/bge-m3' as embedding model and 'mistralai/Mistral-7B-Instruct-v0.3' as the main LLM) and libraries such as langchain and faiss.

## instructions
If you would like to run the model on your personal computer, I need to give you a peace of advice. Firstly, get your token on https://huggingface.co/settings/tokens, then copy and paste them into 'global variables' inside .ipynb file. To provide the model with processed documents you need to upload .zip file to .ipynb while running the code.
