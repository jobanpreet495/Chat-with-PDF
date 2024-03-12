# Chat-with-PDF
Chat with PDF using OpenAI  , LangChain . User interface is developed using streamlit

How it works:
User upload the PDF file
Content is extracted from the PDF file and splitted into chunks.
Embeddings are created of those text chunks and stored in a Knowledge base which is in our case is FAISS 
FAISS : facebook AI similarity search is a library used for similarity search.
When user ask a question , it firstly converted to embeddings and then sematic search is applied to extract relevant chucnk from the knowledge base .
This chunk and question is then passed to the llm (Which in our case is OpenAI gpt model) to get relevant answer.
