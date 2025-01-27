# LangChain-Integrated RAG Framework with Groq Gemma2-9b-it and Llama Embeddings for Contexualized Document Synthesis
<p align="center">
  <img src="https://github.com/user-attachments/assets/babaafbb-11a0-48c3-b262-27694c41bcd3" alt="Image" width="500">
</p>

## Project Overview
This project implements a Retrieval-Augmented Generation (RAG) framework using LangChain and the Groq Gemma2-9b-it model with llama embeddings. The aim is to create a highly contextualized and efficient system for synthesizing responses based on scraped documents from web articles. Additionally, a small web application was developed using Streamlit to provide a user-friendly interface for interacting with the RAG system.

## Features
- **Data Scraping**: Web articles were scraped using `UnstructuredURLLoader` to create a dataset of unstructured text.
- **LangChain Framework**: Built a modular LangChain pipeline for seamless integration with multiple components.
- **Groq Gemma2-9b-it Model**: Utilized the Gemma2-9b-it model through Groq's API for generating contextually enriched responses.
- **Llama Embeddings**: Leveraged pretrained llama embeddings to improve the quality of document similarity and relevance scoring in the RAG framework.
- **Retrieval-Augmented Generation (RAG)**: Integrated the retrieval mechanism for fetching relevant chunks of documents to provide accurate responses to user queries.
- **Streamlit Web Application**: A lightweight and interactive web app was developed to make the RAG framework accessible via a user-friendly interface.

## Workflow
1. **Data Collection**:
   - Articles were scraped from specified URLs using a custom user-agent header for better compatibility.
   - The `UnstructuredURLLoader` from LangChain was employed to parse and preprocess the scraped text.
   
2. **Embedding Generation**:
   - Used llama embeddings to encode the document chunks for efficient similarity matching.
   
3. **Model Integration**:
   - Connected to the Groq Gemma2-9b-it model via its API using `ChatGroq`.
   - Customized the temperature setting to control response diversity.

4. **RAG Pipeline**:
   - Integrated retrieval and generation by combining embeddings and Groq's LLM to generate context-aware responses.
   - Tested the pipeline by posing queries and observing the system's ability to retrieve and synthesize information from the scraped articles.

5. **Web Application**:
   - A web app was developed using Streamlit and VS Code to make the RAG system interactive.
   - The app allows users to input queries, retrieve relevant document chunks, and receive generated responses in real time.

## Tools and Libraries
- **LangChain**: Framework for building RAG pipelines and chaining LLMs.
- **Groq Gemma API**: API for accessing the Gemma2-9b-it model for generation tasks.
- **Llama Embeddings**: Pretrained embedding model for semantic similarity scoring.
- **Unstructured**: Used for extracting text data from unstructured web sources.
- **Streamlit**: Framework for creating the interactive web application.
- **VS Code**: Code editor used for developing and debugging the project.
- **Python**: Programming language used to integrate all components.
