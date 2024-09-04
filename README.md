# Question-Answer-AI
Welcome to PDF Query Assistant, a handy tool that empowers users to ask questions about PDF documents and receive accurate answers. This file provides an overview of the project, its features, and instructions for usage.Here id the process design for the same: 
![image](https://github.com/user-attachments/assets/ad5b9300-6dc3-4187-b1c0-ac2574a6210e)

## System Flow/Architechture 

The system is designed to process and respond to user queries by:
1. Extracting Information: The system can extract text from uploaded PDF documents.
2. Text Chunking: The extracted text is divided into smaller, manageable chunks.
3. Embedding Creation: Each chunk of text is converted into vector embeddings using OpenAI’s language models, which are representations that the AI can understand and work with.
4. Storing Data: The vector embeddings are stored in Pinecone, a vector database designed for similarity searches.
5. User Interaction: Users interact with the system through a Streamlit interface, where they can ask questions and receive answers. The system searches for relevant information using the embeddings and generates responses with the help of OpenAI’s language model.
6. History and Storage: All interactions (questions and responses) are stored in Firebase, which allows the system to maintain context and recall past conversations.
![image](https://github.com/user-attachments/assets/53a8df7f-f63d-4942-8d8e-90f227b5d5bc)

## Features
Upload PDF: Users can easily upload their PDF files through the user-friendly interface.

Ask Questions: Once the PDF is uploaded, users can ask questions related to the content of the document.

Intelligent Query Assistant: The system uses advanced natural language processing to understand and analyze the questions, providing relevant and precise answers.

User-Friendly Interface: The interface is designed for simplicity, ensuring a seamless and intuitive experience for users.

## Tech Stack: 
Python

Streamlit

Langchain

Pinecone

Firebase

HTML

CSS

## API used:
OpenAI 

Pinecone

## Getting Started

1. Clone the project repository
2. Create python environment
3. Install  dependencies using the provided requirements.txt file:
     pip install -r requirements.txt
4. Obtain OpenAI API key and add in .env file
5. Create Index in Pinecone with deimnsions 1536
6. Add Pinecone API key, enviorment key and index name in main.py file
7. Create project in Firebase and add the Database url and .json file path in main.py file
8. Run the application in you environment using:
       streamlit run main.py

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
Special thanks to the contributors and the open-source community for their valuable input and support.

Happy querying! 🚀
