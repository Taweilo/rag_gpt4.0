# rag with gpt4.0
<img src="https://github.com/user-attachments/assets/34f71e70-78eb-4768-a629-58812cdd2bcf" width="800">

## Dependency
- gradio
- langchain
- openai
- faiss-cpu
- pypdf

## Steps
1. Upload a PDF document.
2. Process the PDF to extract and embed its content using FAISS.
3. Use GPT-4.0 as the LLM to answer questions based on the document.
4. Chat with the document using a conversational interface.

## Code - How to Use It
The main components of the code include:
- process_pdf(pdf_file): Extracts text from the uploaded PDF, splits it into chunks, and stores it in a FAISS vector database.
- chatbot(query, chat_history): Handles user queries by retrieving relevant document chunks and generating responses using GPT-4.0.
- A Gradio interface with file upload, chat history, and example queries.

1. Run the script in a Python environment with the required dependencies installed.
2. Upload a PDF file via the Gradio interface.
3. Click the "Process PDF" button to extract and index the document.
4. Enter your questions in the chat interface to interact with the document.

## Further Advancement
1. Deployment: Deploy as a web app using platforms like Hugging Face Spaces or Streamlit Sharing.
2. Free LLM: Explore alternative LLMs such as OpenAssistant or Hugging Face Transformers to avoid OpenAI API costs.
3. Vector Store: Experiment with other vector databases like ChromaDB or Pinecone for scalability and better retrieval.
