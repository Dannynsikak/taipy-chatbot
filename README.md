## StackUp Assistant

StackUp Assistant is an intelligent chatbot application built using LangChain, Taipy, and Google Generative AI. It leverages advanced language models and vector-based search to provide meaningful and contextual responses based on FAQ documents.

Features
FAQ Processing: Reads and processes text files from a specified folder.
Vector-based Search: Uses vector-based document retrieval for efficient querying.
Generative AI Responses: Leverages Google Generative AI for advanced conversational capabilities.
User-friendly GUI: Built using Taipy for an interactive and dynamic user interface.
New Conversations: Easily reset the conversation for a fresh start.
Prerequisites
Ensure the following are installed before running the project:

Python 3.8 or later
Required libraries (install via pip install -r requirements.txt):
langchain
taipy
pandas
python-dotenv
langchain-community
langchain-huggingface
langchain-google-genai
FAQ text files placed in the ./data directory.
Getting Started

1. Clone the Repository

   git clone https://github.com/your-username/stackup-assistant.git
   cd stackup-assistant

2. Install Dependencies

   pip install -r requirements.txt

3. Configure Environment Variables
   Create a .env file in the root directory and specify your credentials:

env

GOOGLE_GENAI_API_KEY=your_google_genai_api_key 4. Add FAQ Data
Place your .txt FAQ files in the ./data directory. Ensure they are well-structured and formatted for effective indexing.

5. Run the Application
   Run the Python script:

python app.py
Access the GUI in your browser at[Browser-port](http://localhost:5000).

Code Overview
Main Components
Environment Variables: Loaded via dotenv for secure API key management.
FAQ Indexing:
Loads .txt files from the ./data folder.
Creates a vector-based index using LangChain’s VectorstoreIndexCreator with HuggingFace embeddings.
Generative AI:
Utilizes Google’s Generative AI (Gemini 1.5) for generating contextual responses.
Dynamic GUI:
Designed using Taipy GUI Builder for an interactive user interface.
Chat Functions:
send_message: Handles user input, queries the LLM, and updates the conversation state.
reset_chat: Clears the chat and starts a new conversation.
Folder Structure

stackup-assistant/
│
├── data/ # Folder for FAQ text files
├── app.py # Main application code
├── requirements.txt # List of dependencies
└── .env # Environment variables (not included in Git)
GUI Design
Sidebar: Contains the "New Conversation" button.
Chat Area: Displays conversation history with the assistant.
Message Input: Allows users to input their queries.
Example Interaction
Start the Application: Open the GUI.
Ask a Question: Type your question in the input field and hit Enter.
Get Responses: View contextual responses from the assistant.
New Conversation: Click "New Conversation" to reset the chat.
Future Enhancements
Add support for additional file formats (e.g., PDFs, Word documents).
Extend the chatbot’s capabilities to handle multi-turn conversations.
Enhance GUI design with more customization options.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
For questions, suggestions, or contributions, feel free to contact:

Email: nsikakdanny11@gmail.com
GitHub: [your-username](https://github.com/Dannynsikak)
