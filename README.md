# DocuMind AI 🔍

DocuMind AI is an intelligent document analysis application that enables users to chat with their PDF documents using advanced RAG (Retrieval-Augmented Generation) technology.

## Features

- **PDF Document Processing**: Upload and index your PDF documents for intelligent retrieval
- **Interactive Chat Interface**: Ask questions about your documents and receive comprehensive answers
- **Knowledge Base Integration**: Automatic creation of a searchable knowledge base from your PDFs
- **Smart RAG Agent**: Uses OpenAI's models to provide contextually relevant responses
- **External Search Integration**: Falls back to DuckDuckGo search when additional information is needed
- **Citation Precision**: Provides page numbers and section headers in responses
- **Markdown Formatting**: Well-structured responses with appropriate formatting
- **PDF Preview**: View your document directly in the application

## Technology Stack

- **Frontend**: Streamlit
- **AI Models**: OpenAI GPT models (gpt-4o-mini default)
- **Embeddings**: OpenAI Embeddings
- **Vector Database**: Milvus
- **RAG Framework**: Agno library for knowledge base creation and agent management

## Architecture Workflow
![Workflow](https://github.com/ShikharPatelNEU/Docu-Mind-AI/blob/main/documind_ai_flow.png)

## Setup and Installation

1. Clone this repository
2. Install dependencies:
3. Set up environment variables:
- `OPENAI_API_KEY`: Your OpenAI API key
- `MILVUS_URI`: URI for Milvus vector database (default: http://localhost:19530)

4. Run the application:

## Usage

1. Upload a PDF document using the sidebar
2. Click "Process Document" to index your document
3. Start asking questions in the chat interface
4. Receive comprehensive answers based on the document content

## Agent Capabilities

The RAG agent is configured to:
- Search the knowledge base first for every query
- Use external search when necessary
- Provide specific citations and sources
- Structure responses with clear formatting
- Ask for clarification on ambiguous queries
- Suggest related topics or follow-up questions
