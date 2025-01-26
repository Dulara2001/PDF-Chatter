# PDF Chatter: Chatbot with PDF Integration

**Demo** : https://drive.google.com/file/d/1YBuxinEQnDV8rLmrChhmdVIbwKQ3PcUT/view?usp=sharing

**PDF Chatter** is an innovative LLM application that allows users to interact with the content of PDF documents using a chatbot interface. The application leverages **Google gemini pro**, a powerful language model, to provide intelligent, context-aware responses based on the content extracted from the provided PDF file. Whether you’re looking to summarize a document, answer specific questions, or gain insights from lengthy text, **PDF Chatter** makes it easier and faster by allowing you to interact with PDF data naturally.

## Technologies

- **Python**: The primary programming language used for implementing the core functionality of the application.
- **LangChain**: A framework used to connect different components like embeddings, vector stores, and language models, facilitating document-based question-answering.
- **FAISS**: A vector store for efficient similarity search, enabling fast retrieval of relevant information from the PDF content.
- **Streamlit**: A framework to create the user interface for easy interaction with the PDF and chatbot system.
- **PyPDF2**: A Python library to extract text from PDF files.
- **Google gemini pro**: A next-gen AI language model used to provide intelligent and contextually accurate answers based on the PDF content.
  
## Key Features

- **PDF Interaction**: Upload and interact with the content of any PDF file.
- **Context-Aware Question-Answering**: Ask specific questions about the PDF, and get accurate answers derived directly from its content.
- **Real-Time Responses**: Instant interaction with the chatbot for efficient reading and understanding of PDF documents.
- **Vector Search with FAISS**: FAISS is used to index and perform fast similarity searches for efficient querying of relevant text from the PDF.
- **Secure Deserialization**: Pickle files are deserialized securely to avoid malicious code execution, with an option to enable deserialization only if the source is trusted.

## Architecture

- **Text Extraction**: The PyPDF2 library extracts text from the uploaded PDF.
- **Text Chunking**: The extracted text is divided into manageable chunks for better processing.
- **Embedding Generation**: Text chunks are embedded into vectors using a chosen embedding model.
- **Vector Search with FAISS**: FAISS indexes the vector embeddings and performs efficient searches to match user queries to relevant text.
- **Question Answering with Gemini**: Gemini generates context-aware answers based on the query and relevant text retrieved from the PDF.
