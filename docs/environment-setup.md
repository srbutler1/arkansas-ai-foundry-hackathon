# Environment Setup Guide

This guide will help you set up your development environment for the Arkansas AI Foundry Hackathon.

## Python Setup

### 1. Install Python

We recommend using Python 3.8 or newer.

#### Windows
- Download the installer from [python.org](https://www.python.org/downloads/)
- During installation, make sure to check "Add Python to PATH"

#### macOS
- Using Homebrew: `brew install python`
- Or download from [python.org](https://www.python.org/downloads/)

#### Linux
- Ubuntu/Debian: `sudo apt update && sudo apt install python3 python3-pip`
- Fedora: `sudo dnf install python3 python3-pip`

### 2. Set Up a Virtual Environment

Virtual environments help you manage dependencies for different projects.

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

## Git Setup

### 1. Install Git

#### Windows
- Download and install from [git-scm.com](https://git-scm.com/download/win)

#### macOS
- Using Homebrew: `brew install git`
- Or download from [git-scm.com](https://git-scm.com/download/mac)

#### Linux
- Ubuntu/Debian: `sudo apt install git`
- Fedora: `sudo dnf install git`

### 2. Configure Git

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## IDE Recommendations

Choose an IDE or code editor that you're comfortable with:

- **Windsurf**: The world's first agentic IDE with powerful AI-assisted coding capabilities
  - Install from [codeium.com/windsurf](https://www.codeium.com/windsurf)

- **Visual Studio Code**: Free, lightweight, and has excellent Python support
  - Install from [code.visualstudio.com](https://code.visualstudio.com/)
  - Recommended extensions: Python, Pylance, Jupyter

- **Cursor**: AI-native code editor built for pair programming
  - Install from [cursor.sh](https://cursor.sh/)

## Setting Up Common AI Libraries

### Basic Data Science Stack

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Deep Learning Frameworks

```bash
# TensorFlow
pip install tensorflow

# PyTorch
pip install torch torchvision torchaudio
```

### Natural Language Processing

```bash
pip install transformers datasets nltk spacy
python -m spacy download en_core_web_sm
```

### Computer Vision

```bash
pip install opencv-python pillow
```

### LLM & Generative AI

```bash
# Core LLM tools
pip install langchain openai

# Open Source AI Tools
pip install privateGPT docsgpt autogpt
```

## Open Source AI Tools Setup

### Local LLM Setup

Setting up local LLMs for privacy-focused applications:

```bash
# Clone LocalAI repository
git clone https://github.com/go-skynet/LocalAI
cd LocalAI

# Follow the setup instructions in the repository README
# This provides a local alternative to OpenAI API
```

### Document Processing

For working with document-based applications:

```bash
# Clone pdfGPT for document question-answering
git clone https://github.com/bhaskatripathi/pdfGPT
cd pdfGPT

# Install dependencies
pip install -r requirements.txt
```

### Autonomous AI Agents

For building autonomous AI agents:

```bash
# SuperAGI - Open source autonomous AI agent framework
git clone https://github.com/TransformerOptimus/SuperAGI
cd SuperAGI

# Follow installation instructions in the repository
```

### Audio Processing

For audio generation and processing:

```bash
# Facebook's Audiocraft
git clone https://github.com/facebookresearch/audiocraft
cd audiocraft
pip install -e .
```

## Cloud Platform Setup (Optional)

If you plan to use cloud resources:

### Google Colab
- No setup required, just visit [colab.research.google.com](https://colab.research.google.com/)

### Hugging Face Spaces
- Create an account at [huggingface.co](https://huggingface.co/)

### AWS/Azure/GCP
- Follow the respective cloud provider's documentation for setting up accounts and CLI tools

## Docker (Optional)

If you want to containerize your application:

```bash
# Install Docker from docker.com

# Run a basic Python container
docker run -it --rm python:3.9 python -c "print('Hello from Docker!')"
```

## Troubleshooting

### Common Issues

1. **"Python not found" or "pip not found"**
   - Make sure Python is added to your PATH
   - Try using `python3` and `pip3` instead

2. **Permission errors when installing packages**
   - On Linux/macOS, use `sudo pip install` or set up a virtual environment
   - On Windows, run Command Prompt as Administrator

3. **Package conflicts**
   - Always use a virtual environment
   - Consider using `pip freeze > requirements.txt` to document your dependencies

### Getting Help

If you encounter issues:
- Check the documentation for the specific tool or library
- Search on Stack Overflow
- Ask in our hackathon Discord/Slack channel

## Next Steps

Once your environment is set up:
1. Clone the hackathon repository
2. Explore the example projects
3. Start building your own solution!

Happy coding!
