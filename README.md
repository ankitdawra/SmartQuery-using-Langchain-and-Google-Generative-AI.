# SmartQuery-using-Langchain-and-Google-Generative-AI.
This Notebook demonstrates how to build a question-answering system using Langchain and Google Generative AI.


### Implementation Details

1.	**Install Libraries** - Necessary libraries like PyPDF2, Langchain, FAISS, ConversationBufferMemory etc are installed.
3.	**Extract Text**: Text is extracted from a PDF file named '**AssignmentSupportDocument.pdf**' using PyPDF2.
4.	**Split Text**: The extracted text is split into smaller chunks for efficient processing using **RecursiveCharacterTextSplitter**.
5.	**Generate Embeddings**: Embeddings are generated for each text chunk using GoogleGenerativeAIEmbeddings.
6.	**Create Vector Store**: A FAISS vector store is created and populated with the text chunks and their embeddings.
7.	**Query and Answer**: A loop allows users to input queries. For each query:


        - Relevant text chunks are retrieved from the vector store.
  	    - A Google Generative AI model is used to generate an answer based on the retrieved chunks through RetrievalQAWithSourcesChain.
  	    - The answer is printed to the console.


### High level Architecture
![image](https://github.com/user-attachments/assets/7f4bc302-a9d6-4a7c-8d66-98e7a2bc266a)

 
### Execution instructions
Copy the python file and run it simply in the jupyter notebook.


