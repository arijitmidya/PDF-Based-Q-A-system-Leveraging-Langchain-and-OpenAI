# PDF-Based-Q-A-system-Leveraging-Langchain-and-OpenAI

Objective : 
The objective is to build a Q & A system based on PDF's uploaded . The workflow includes uplading multiple PDF's and asking questions from it .

High Level architecture : ![image](https://github.com/user-attachments/assets/5914be65-fb31-4086-b1f3-df9c6403a438)


Code Explanation : 

1. The PDF files can be uploaded using a file_uploader function
2. The get_pdf_text function Extracts text from a list of PDF documents and returns a single string
3. The get_text_chunks function splits a given text into smaller chunks of a specified size with overlapping sections to maintain context.
4. The get_vectorstore function creates a vector store using OpenAI embeddings to represent text chunks, enabling efficient similarity search.
5. The get_conversation_chain function creates a conversational chain using a language model and a vector store, enabling the model to access and utilize relevant information from the vector store to generate more informative and contextually relevant responses.
6. The handle_userinput function processes user input, updates the chat history, and displays the conversation history using formatted templates.

Implementation : 

Step 1 : Replicate the folder structure

Step 2 : Run the requirements.txt file ( command : pip install -r requirements.txt )

Step3 : Update the .env file with your respective OpenAI keys

Step 4 : Update the images as per your convenience with bot_template and user_template in htmlTemplates.py

![image](https://github.com/user-attachments/assets/473b8873-65a2-48d3-a412-b0849e5f5c0d)


Step 5 : Run the streamlit app locally ( command : streamlit run app.py )

Screenshots from my Run : 

![image](https://github.com/user-attachments/assets/3be12e9b-aa4a-4f47-a382-24824fd0750b)

![image](https://github.com/user-attachments/assets/df4b865d-9e7a-410d-8869-0ac14a2583bb)

![image](https://github.com/user-attachments/assets/706a0b0d-03a0-43f8-81fd-110acec27f29)

![image](https://github.com/user-attachments/assets/244fa880-cfb1-4f75-8745-b87866de35a4)

![image](https://github.com/user-attachments/assets/fcaadfe8-7d0a-4439-bf2f-76fce09ebee2)

Happy coding :) 





















