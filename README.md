# AI-Powered College Chatbot using Retrieval-Augmented Generation (RAG)
<img width="600" height="336" alt="image" src="https://github.com/user-attachments/assets/aad76131-9f23-439c-a041-70638858db92" />

This project implements an **AI-powered College Information Chatbot** using **Retrieval-Augmented Generation (RAG)**.  
The chatbot answers student queries by retrieving information from college documents such as syllabus, academic calendar, and FAQs, and generating accurate, context-based responses using a Large Language Model (LLM).


---

## Project Overview

Traditional chatbots often provide generic or incorrect answers due to lack of contextual grounding.  
This project solves that problem by combining:

- **Document Retrieval (Vector Search)**
- **Large Language Models (LLMs)**
- **Prompt Engineering**

The chatbot retrieves relevant information from college documents and generates **fact-based, context-aware responses**.

---

## Key Concepts Used

- Natural Language Processing (NLP)
- Embeddings & Semantic Search
- Vector Databases (FAISS)
- Large Language Models (LLMs)
- Retrieval-Augmented Generation (RAG)
- Prompt Engineering

---

## I. Setup and Data Preparation
**Import Libraries:**  
Required Python libraries are imported to support document loading, text processing, embeddings, and language model interaction.

**Loading the Data:**  
College-related documents (PDFs) are loaded as the knowledge base for the chatbot.

**Data Preprocessing:**  
Text is extracted from PDFs, cleaned, and prepared for further processing.

**Text Chunking:**  
The processed text is split into smaller chunks to improve retrieval accuracy and handle LLM token limitations.

---

## II. Text Processing
**Embedding Generation:**  
Each text chunk is converted into a vector embedding that captures its semantic meaning.

**Vector Database Creation:**  
All embeddings are stored in a FAISS vector database to enable fast similarity-based retrieval.

---

## III. Query Handling and Retrieval
**User Query Processing:**  
User queries are converted into embeddings and matched with relevant document chunks from the vector database.

**Context Construction:**  
The retrieved document chunks are combined to form contextual input for the language model.

---

## IV. Model Inference
**Large Language Model (LLM):**  
The LLM generates answers strictly based on the retrieved context using a structured prompt, reducing hallucinations.

---

## V. Conclusion
This project demonstrates an end-to-end **RAG-based Generative AI system**, integrating NLP, embeddings, vector databases, and LLMs to deliver accurate college-related information. It is suitable for academic evaluation and real-world applications.



