# Pdf_Chatbot

A powerful PDF document interaction tool that allows users to have conversations with their PDF documents using Google's Generative AI (Gemini). Built with Streamlit and LangChain, this application provides an intuitive interface for uploading PDFs and asking questions about their content.

## Features

- 📁 Multiple PDF file upload support
- 💬 Interactive chat interface
- 🔍 Intelligent text chunking and processing
- 🧠 Powered by Google's Gemini AI model
- 📊 Vector store implementation using FAISS
- 🎯 Accurate context-based responses

## Prerequisites

- Python 3.7+
- Google API key for Gemini

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd pdf-chatbot
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the root directory and add your Google API key:
```
GOOGLE_API_KEY=your_api_key_here
```

## Required Dependencies

```
streamlit
PyPDF2
langchain
faiss-cpu
google-generativeai
python-dotenv
```

## Usage

1. Start the application:
```bash
streamlit run app2.py
```

2. Open your web browser and navigate to the provided local URL (typically `http://localhost:8501`)

3. Using the application:
   - Upload one or more PDF files using the sidebar
   - Click "Submit & Process" to process the documents
   - Type your questions in the input field
   - Get AI-powered responses based on the content of your PDFs

## How It Works

1. **PDF Processing**: The application extracts text from uploaded PDF files
2. **Text Chunking**: The extracted text is split into manageable chunks
3. **Vector Storage**: Text chunks are converted into vectors using Google's embedding model
4. **Question Answering**: User queries are processed using a conversational chain with Gemini
5. **Response Generation**: The system provides detailed answers based on the PDF content

## Features in Detail

- **Multiple PDF Support**: Upload and process multiple PDF documents simultaneously
- **Contextual Understanding**: The system maintains context while answering questions
- **User-Friendly Interface**: Clean and intuitive Streamlit-based web interface
- **Efficient Processing**: Uses FAISS for fast and efficient similarity search
- **Smart Chunking**: Implements recursive character text splitting for optimal processing

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Built with Streamlit
- Powered by Google's Generative AI
- Uses LangChain for LLM interactions
- FAISS for vector storage
