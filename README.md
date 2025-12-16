# MediChat – GenAI Medical Document Assistant

A Streamlit-based GenAI application that allows users to upload medical PDFs and ask questions using RAG (Retrieval-Augmented Generation).

⚠️ Disclaimer: This tool does not provide medical advice.

## Tech Stack
- Python 3.11
- Streamlit
- LangChain
- FAISS
- Sentence Transformers

### 🔁 How Retrieval-Augmented Generation (RAG) Works

1. Users upload medical PDF documents through the Streamlit interface.
2. The uploaded PDFs are parsed and converted into raw text using PDF utilities.
3. The extracted text is split into overlapping chunks using `RecursiveCharacterTextSplitter` to preserve context.
4. Each text chunk is converted into dense vector embeddings using Sentence Transformers.
5. The embeddings are stored inside a FAISS vector index for efficient similarity search.
6. When a user submits a query, FAISS retrieves the most semantically relevant document chunks.
7. The retrieved context is passed to the Large Language Model via LangChain.
8. The LLM generates a grounded response strictly based on the retrieved document context.
9. The final answer is displayed back to the user in the Streamlit UI.

This RAG-based approach minimizes hallucinations and ensures responses are derived from the uploaded medical documents.

---
