<a href="https://colab.research.google.com/drive/15EOwhz7qRVrAXw6NLy_GlGfUaKAqSMfX?usp=sharing">Colab Link</a>

<h2>Retrieval Augmented Generation with LangChain</h2>
<b>Made using IBM cloud</b>
<P>RAG is an architectural pattern that can be used to augment the performance of language models by recalling factual information from a knowledge base, and adding that information to the model query. The most common approach in RAG is to create dense vector representations of the knowledge base in order to retrieve text chunks that are semantically similar to a given user query.</P>

---

## 📖 Overview

RAG enhances the capabilities of language models by incorporating factual information from a **knowledge base** into the response generation process.  
In this project, documents are embedded, stored in a **vector database**, and retrieved at query time to provide relevant context to the model.

---

## ⚙️ How It Works

The RAG process in this implementation consists of three main steps:

1. **Initial Setup**
   - Convert documents into embeddings.
   - Store embeddings in a **vector database** for fast similarity search.

2. **On Each User Query**
   - Embed the query.
   - Retrieve semantically similar document chunks from the database.

3. **Generate Response**
   - Combine the retrieved context with the query.
   - Use **IBM Granite LLM** via LangChain to produce a grounded answer.

---


