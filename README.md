# 🤖 CodeQwen Interactive Chat System

A modern, AI-powered interactive code generation and conversation system built with Hugging Face's CodeQwen model and Gradio. Features real-time streaming responses, multi-language code conversion, and a beautiful cyberpunk-inspired UI.

![CodeQwen Banner](https://img.shields.io/badge/AI-CodeQwen-00d4ff?style=for-the-badge&logo=artificial-intelligence)
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)
![Gradio](https://img.shields.io/badge/Gradio-4.0+-orange?style=for-the-badge&logo=gradio)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

## 🚀 Features

### 🎯 Core Capabilities
- **Interactive Code Generation** - Generate code in multiple programming languages
- **Real-time Streaming** - Watch responses appear word-by-word as they're generated
- **Language Conversion** - Convert code between different programming languages
- **Code Explanation** - Get detailed explanations of code functionality
- **Performance Optimization** - Optimize code for better performance
- **Chat History** - Persistent conversation history with context awareness

### 🎨 User Interface
- **Modern Cyberpunk Design** - Sleek dark theme with neon accents
- **Glassmorphism Effects** - Translucent elements with blur effects
- **Responsive Layout** - Works seamlessly on desktop and mobile
- **Animated Elements** - Smooth transitions and glowing effects
- **Professional Typography** - JetBrains Mono for code, Inter for UI

### ⚡ Advanced Features
- **Multi-model Support** - Framework ready for multiple AI models
- **Temperature Control** - Adjust AI creativity and randomness
- **Session Statistics** - Track messages and token usage
- **Export Functionality** - Save chat history to text files
- **Quick Examples** - Pre-built prompts for common tasks

## 🛠️ Installation

### Prerequisites
- Python 3.8 or higher
- CUDA-compatible GPU (recommended for better performance)
- 8GB+ RAM (16GB+ recommended)

### Quick Setup

1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/codeqwen-interactive-chat.git
cd codeqwen-interactive-chat
```

2. **Create a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Run the application:**
```bash
python app.py
```

5. **Open in browser:**
   - Local: `http://localhost:7860`
   - Public URL will be displayed in terminal (if sharing is enabled)

## 🎮 Usage

### Basic Chat
1. Type your coding question or request in the input field
2. Click "Send ⚡" or press Enter
3. Watch the AI response stream in real-time
4. Continue the conversation with context awareness

### Quick Examples
Use the pre-built example buttons for common tasks:
- **🐍 Python Sorting Algorithm** - Generate sorting implementations
- **🔄 Python ➜ JavaScript** - Convert between languages
- **🔍 Explain Recursion** - Get detailed explanations
- **🌐 Flask REST API** - Create web APIs
- **⚡ Optimize Performance** - Improve code efficiency
- **🛠️ Debug Code** - Fix and debug issues

### Advanced Settings
- **🌊 Enable Streaming** - Toggle real-time response streaming
- **🌡️ Temperature** - Control AI creativity (0.1-1.0)
- **🎯 Model Selection** - Choose between different AI models
- **📊 Session Stats** - Monitor usage statistics

## 🔧 Configuration

### Model Settings
```python
# Default model configuration
MODEL_NAME = "Qwen/CodeQwen1.5-7B-Chat"
MAX_NEW_TOKENS = 1024
TEMPERATURE = 0.7
TOP_P = 0.9
```

### UI Customization
- Modify `custom_css` in the code to change colors and styling
- Adjust `height` and `scale` parameters for layout changes
- Customize example buttons and prompts

### Environment Variables
Create a `.env` file for sensitive configurations:
```env
MODEL_CACHE_DIR=./models
GRADIO_SERVER_NAME=0.0.0.0
GRADIO_SERVER_PORT=7860
```

## 🏗️ Project Structure

```
codeqwen-interactive-chat/
├── app.py                 # Main application file
├── requirements.txt       # Python dependencies
├── README.md             # This file
├── .env.example          # Environment variables template
├── .gitignore           # Git ignore rules
├── models/              # Model cache directory
├── exports/             # Exported chat histories
└── static/              # Static assets (if any)
```

## 🤝 Contributing

We welcome contributions! Here's how to get started:

1. **Fork the repository**
2. **Create a feature branch:**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make your changes and test**
4. **Commit your changes:**
   ```bash
   git commit -m "Add amazing feature"
   ```
5. **Push to the branch:**
   ```bash
   git push origin feature/amazing-feature
   ```
6. **Open a Pull Request**

### Development Guidelines
- Follow PEP 8 coding standards
- Add docstrings to all functions
- Include type hints where appropriate
- Test your changes thoroughly
- Update documentation as needed

## 📝 Examples

### Code Generation
```
User: Create a Python function to calculate Fibonacci numbers
AI: Here's an efficient Python implementation with memoization...
```

### Language Conversion
```
User: Convert this Python code to JavaScript: def greet(name): return f"Hello, {name}!"
AI: Here's the JavaScript equivalent: function greet(name) { return `Hello, ${name}!`; }
```

### Code Explanation
```
User: Explain how bubble sort works
AI: Bubble sort is a simple sorting algorithm that works by repeatedly stepping through the list...
```

## 🐛 Troubleshooting

### Common Issues

**1. Model Loading Errors**
```bash
# Clear model cache
rm -rf ~/.cache/huggingface/transformers/
```

**2. CUDA Out of Memory**
```python
# Reduce batch size or max tokens
MAX_NEW_TOKENS = 512
```

**3. Gradio Port Issues**
```bash
# Try different port
python app.py --port 7861
```

**4. Slow Response Times**
- Ensure GPU is being used
- Reduce model precision to fp16
- Close other GPU-intensive applications

## 📋 System Requirements

### Minimum Requirements
- **CPU:** 4-core processor
- **RAM:** 8GB
- **Storage:** 10GB free space
- **GPU:** Optional but recommended

### Recommended Requirements
- **CPU:** 8-core processor
- **RAM:** 16GB+
- **Storage:** 20GB+ SSD
- **GPU:** NVIDIA RTX 3060 or better

## 🔐 Security Notes

- Model runs locally - your code never leaves your machine
- No data is sent to external servers
- Chat history is stored locally
- Consider using environment variables for sensitive configs

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Qwen Team** for the amazing CodeQwen model
- **Hugging Face** for the transformers library
- **Gradio Team** for the awesome UI framework
- **Open Source Community** for inspiration and contributions

## 📞 Support

- **Issues:** [GitHub Issues](https://github.com/Atharvax/codeqwen-interactive-chat/issues)
- **Discussions:** [GitHub Discussions](https://github.com/Atharvax/codeqwen-interactive-chat/discussions)
- **Email:** atharvakocharekar0@gmail.com

## 🔄 Updates

### Version 1.0.0 (Current)
- Initial release with CodeQwen integration
- Streaming response support
- Modern UI with cyberpunk theme
- Multi-language code conversion
- Export functionality

### Planned Features
- [ ] Multi-model support (Llama, Mistral, etc.)
- [ ] Code execution environment
- [ ] Plugin system
- [ ] Collaborative features
- [ ] Advanced code analysis
- [ ] Custom model fine-tuning

---

<div align="center">

**⭐ Star this repo if you found it helpful!**

Made with ❤️ by [Atharvax]

</div>
