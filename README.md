# DocQuery: PDF Document Querying with FAISS and Google Generative AI
**DocQuery** is a powerful tool for querying information from PDF files using state-of-the-art AI embeddings and the FAISS vector store. With this app, you can upload multiple PDF files, process them into searchable text chunks, and ask questions to extract detailed answers from the documents.

**Key Features:**
PDF Text Extraction: Upload multiple PDF files, and the tool will extract and process text from each page.
Efficient Text Chunking: Uses LangChain's RecursiveCharacterTextSplitter to break down large documents into manageable text chunks.
Vector Store Search: Implements FAISS (Facebook AI Similarity Search) to create a searchable vector store of the PDF content.
Google Generative AI Embeddings: Leverages Google Generative AI for high-quality embeddings of text chunks.
Conversational AI: Uses LangChain's ChatGoogleGenerativeAI to answer user questions based on the content of the uploaded PDFs. The system ensures answers are derived strictly from the document context.
Streamlit Interface: A user-friendly interface built with Streamlit that allows you to upload PDFs, ask questions, and receive AI-generated answers.
How It Works:
Upload one or more PDF files.
The app processes the text and stores embeddings in a FAISS vector store.
Ask questions about the documents, and the AI retrieves relevant information, providing detailed answers.
If the answer to a question isn't in the document, the AI will indicate that no information is available.

**Requirements:**
Streamlit
LangChain
PyPDF2
Google Generative AI SDK
FAISS

**Setup:**
Clone the repository.
Install the required packages using pip.
Set up your Google API key in the .env file.
Run the Streamlit app: streamlit run app.py.