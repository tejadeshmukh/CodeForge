# 🤖 AI Code Generator

**AI Code Generator** is an intelligent multi-agent system that transforms natural language descriptions into complete, working software projects. Built with cutting-edge AI technologies including [LangGraph](https://github.com/langchain-ai/langgraph) and powered by advanced language models.

## ✨ Features

- 🧠 **Intelligent Planning**: Analyzes requirements and creates comprehensive project blueprints
- 🏗️ **Smart Architecture**: Breaks down complex projects into manageable implementation tasks  
- 💻 **Automated Coding**: Generates complete, working code with proper file structure
- 🔧 **Tool Integration**: Uses real developer tools for file management and project setup
- 🛡️ **Secure Execution**: Sandboxed environment prevents unauthorized file access

## 🏗️ System Architecture

The system employs a sophisticated **3-agent workflow** that mimics professional development teams:

- **🧠 Planner Agent** – Analyzes user requirements and generates detailed project specifications
- **🏗️ Architect Agent** – Creates implementation roadmaps with specific engineering tasks
- **💻 Coder Agent** – Executes tasks using developer tools to build complete projects

<div style="text-align: center;">
    <img src="resources/coder_buddy_diagram.png" alt="AI Code Generator Architecture" width="90%"/>
</div>

## 🚀 Quick Start

### Prerequisites
- Python 3.11 or higher
- [uv](https://docs.astral.sh/uv/getting-started/installation/) package manager
- [Groq API key](https://console.groq.com/keys) for AI model access

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ai-code-generator.git
   cd ai-code-generator
   ```

2. **Set up virtual environment**
   ```bash
   uv venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   uv pip install -e .
   ```

4. **Configure environment**
   ```bash
   cp .sample_env .env
   # Edit .env and add your GROQ_API_KEY
   ```

5. **Run the application**
   ```bash
   python main.py
   ```

## 🎯 Example Use Cases

- **Web Applications**: "Create a modern todo app with React and TypeScript"
- **APIs**: "Build a REST API for a blog with FastAPI and PostgreSQL"  
- **Data Projects**: "Generate a data analysis dashboard with Python and Streamlit"
- **Mobile Apps**: "Create a cross-platform app with Flutter"
- **Games**: "Build a simple 2D game with HTML5 Canvas"

## 🔧 Advanced Features

### Multi-Agent Coordination
The system uses LangGraph to orchestrate multiple AI agents, each specialized for different aspects of software development.

### Structured Output
Leverages Pydantic models for reliable data parsing and validation, ensuring consistent project structure.

### Tool Integration
Agents have access to real developer tools:
- File system operations (read/write/list)
- Directory management
- Command execution
- Project structure analysis

### Security First
- Sandboxed file operations
- Path validation to prevent directory traversal
- Controlled tool access

## 📊 Project Structure

```
ai-code-generator/
├── agent/                    # Core AI agent implementations
│   ├── graph.py             # LangGraph workflow orchestration
│   ├── states.py            # Pydantic data models
│   ├── prompts.py           # Agent-specific prompts
│   └── tools.py             # Developer tools integration
├── resources/               # Documentation and diagrams
├── main.py                  # Application entry point
└── pyproject.toml          # Project dependencies
```

## 🛠️ Technology Stack

- **AI Framework**: LangChain + LangGraph
- **Language Model**: Groq (GPT-OSS-120B)
- **Data Validation**: Pydantic
- **Package Management**: uv
- **Environment**: Python 3.11+

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Built with ❤️ by [Your Name]**