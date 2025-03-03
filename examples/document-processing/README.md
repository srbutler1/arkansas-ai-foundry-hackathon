# Document Processing System Example

This example demonstrates how to build an intelligent document processing system using open-source AI tools, inspired by [pdfGPT](https://github.com/bhaskatripathi/pdfGPT).

## Overview

This project showcases how to create a document processing system that can:
- Extract text and data from various document formats (PDF, DOCX, etc.)
- Analyze document content using LLMs
- Answer questions about document content
- Generate summaries and insights

## Technologies Used

This example leverages several open-source AI tools:

- **pdfGPT**: For PDF document question-answering capabilities
- **LangChain**: For document loading, chunking, and processing
- **FAISS/Chroma**: For vector storage and retrieval
- **Streamlit**: For creating a simple UI

## Getting Started

### Prerequisites

- Python 3.8+
- Git
- Basic understanding of document processing and LLMs

### Installation

1. Clone this repository
```bash
git clone https://github.com/YourUsername/arkansas-ai-foundry-hackathon.git
cd arkansas-ai-foundry-hackathon/examples/document-processing
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Set up pdfGPT integration
```bash
git clone https://github.com/bhaskatripathi/pdfGPT
cd pdfGPT
# Follow the setup instructions in the pdfGPT repository
```

4. Run the application
```bash
streamlit run app.py
```

## Project Structure

```
document-processing/
├── app.py                  # Main Streamlit application
├── requirements.txt        # Project dependencies
├── documents/              # Sample documents for testing
│   ├── sample1.pdf         # Sample PDF document
│   ├── sample2.docx        # Sample DOCX document
│   └── sample3.txt         # Sample text document
├── processors/             # Document processing modules
│   ├── pdf_processor.py    # PDF processing utilities
│   ├── docx_processor.py   # DOCX processing utilities
│   └── text_processor.py   # Text processing utilities
├── models/                 # Model integration
│   ├── llm.py              # LLM integration
│   └── embeddings.py       # Document embedding utilities
└── utils/                  # Utility functions
    ├── vectorstore.py      # Vector database functions
    └── preprocessing.py    # Text preprocessing
```

## Customization

To adapt this system for your specific needs:

1. Add custom document processors for specific document types
2. Modify the question-answering pipeline in `models/llm.py`
3. Customize the UI in `app.py`
4. Add additional analytics or export features

## Advanced Features

- **Document Classification**: Automatically categorize documents
- **Information Extraction**: Extract specific fields (dates, names, amounts)
- **Multi-document Analysis**: Compare information across multiple documents
- **Document Summarization**: Generate executive summaries of long documents

## Resources

- [pdfGPT Repository](https://github.com/bhaskatripathi/pdfGPT)
- [LangChain Document Loaders](https://python.langchain.com/docs/modules/data_connection/document_loaders/)
- [FAISS Vector Database](https://github.com/facebookresearch/faiss)

## License

This example is licensed under the MIT License - see the LICENSE file for details.
