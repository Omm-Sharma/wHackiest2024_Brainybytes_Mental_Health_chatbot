# wHackiest2024_Brainybytes_Mental_Health_chatbot
# Mann - Mental Health Support Bot

Mann is a mental health chatbot designed to provide thoughtful and concise responses to mental health-related questions. Built with LangChain, Chroma, HuggingFace embeddings, and Gradio, Mann offers a supportive companion for users in need of guidance and understanding.

---

## Features
- **Compassionate Mental Health Support**: Mann provides empathetic and concise answers to user queries.
- **PDF Knowledge Base**: Upload PDF documents containing mental health information to create a custom knowledge base.
- **Interactive UI**: Easy-to-use interface powered by Gradio.
- **Persistent Storage**: Leverages Chroma for a persistent vector database.
- **Customizable**: Modify the chatbot's behavior, prompt templates, or embeddings as needed.

---

## Installation

### Requirements
- Python 3.8+
- Required libraries: `langchain`, `chromadb`, `gradio`, `sentence-transformers`, `langchain-groq`

### Setup
1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   pip install langchain chromadb gradio sentence-transformers langchain-groq
   ```
3. Set up your environment:
   - Create a `/content/data` directory for uploading PDFs.
   - Replace `GROQ_API_KEY` in the script with your actual Groq API key.

---

## Usage

### Running the Chatbot
1. Place your PDF files containing mental health content in the `/content/data` directory.
2. Run the chatbot script:
   ```bash
   python chatbot.py
   ```
3. Access the chatbot UI through the Gradio interface (a link will appear in the terminal).

### Using the Chatbot
- Type your mental health-related question into the text box and press **Send**.
- Mann will provide a thoughtful, concise response based on the uploaded knowledge base.
- Use the **Clear** button to reset the conversation.

---

## File Structure
```
project-folder/
├── chatbot.py       # Main chatbot script
├── README.md        # Documentation
├── /content/data    # Directory for uploading PDF files
├── /content/chroma_db  # Directory for the persistent vector database
```

---

## Customization

### Adjusting the Model
- Modify the `initialize_llm()` function to change the model configuration.

### Changing the Prompt
- Edit the `prompt_template` in `setup_qa_chain()` to customize how Mann interacts with users.

### Extending the Knowledge Base
- Add more PDFs to the `/content/data` directory and recreate the vector database using the `create_vector_db()` function.

---

## Disclaimer
*Mann is a supportive chatbot and not a licensed therapist. For professional mental health support, please consult a qualified professional.*

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements
- Built with [LangChain](https://www.langchain.com/).
- Embeddings by [HuggingFace](https://huggingface.co/).
- UI powered by [Gradio](https://gradio.app/).
