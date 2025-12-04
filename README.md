# AI-Powered Project Generator

A Streamlit application that uses AI to gather product requirements through interactive chat and automatically generates complete project structures with code files.

## Features

- **Interactive Chat Interface**: Engage with an AI assistant to define your project requirements
- **Intelligent Requirements Gathering**: AI-powered conversation to extract detailed product specifications
- **Automatic Project Generation**: Creates complete folder structures and code files based on requirements
- **GitHub Integration**: Automatically commits and pushes generated projects to GitHub
- **PDF Processing**: Support for document analysis and processing
- **Downloadable Projects**: Generate ZIP files of your complete project

## Tech Stack

- **Frontend**: Streamlit with custom theming
- **AI/ML**: OpenAI GPT models, LangChain
- **Document Processing**: PDFPlumber, PyPDF2, pdfminer.six
- **Version Control**: GitPython integration
- **Data Processing**: Pandas

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd <project-directory>
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
cp example.env .env
# Edit .env with your OpenAI API key and other configurations
```

4. Run the application:
```bash
streamlit run pages/Init_Chat.py
```

## Usage

1. **Start a Conversation**: Begin by describing your project idea in the chat interface
2. **Answer Questions**: The AI will ask clarifying questions to understand your requirements
3. **Review Summary**: Once complete, review the generated product requirements document
4. **Generate Project**: The system automatically creates a complete project structure
5. **Download or Push**: Either download the ZIP file or push directly to GitHub

## Project Structure

```
├── pages/              # Streamlit pages
├── services/           # Business logic and AI processing
├── utils/              # Utility functions
├── exceptions/         # Custom exception handlers
├── renderers/          # UI rendering components
└── .streamlit/         # Streamlit configuration
```

## Configuration

- Copy `example.env` to `.env` and configure your API keys
- Modify `.streamlit/config.toml` for UI theming preferences

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

[Add your license information here]