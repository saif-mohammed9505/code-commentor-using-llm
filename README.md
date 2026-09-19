# 🤖 Code Commentor

An AI-powered Code Commentor that uses Large Language Models (LLMs) to automatically add meaningful comments and explanations to source code.

## ✨ Features

- Automatically adds comments to source code
- Explains code logic and functions
- Explains complex lines and algorithms
- Adds docstrings where appropriate
- Preserves the original code logic
- Detects the programming language
- Beginner-friendly explanations
- Gradio-based user interface
- Supports DeepSeek, Qwen, and Llama 3.2

## 🛠️ Tech Stack

- Python
- OpenAI Python SDK
- Hugging Face Hub
- Ollama
- Gradio
- python-dotenv
- Jupyter Notebook

## 🤖 Models

- DeepSeek: `deepseek-ai/DeepSeek-V3-0324`
- Qwen: `Qwen/Qwen3.5-9B`
- Llama: `llama3.2` through Ollama

## 📂 Project Structure

    Code-Commentor/
    ├── code_commentor.ipynb
    ├── requirements.txt
    ├── .env.example
    ├── .gitignore
    └── README.md

## ⚙️ Installation

### 1. Clone the repository

    git clone https://github.com/YOUR_USERNAME/Code-Commentor.git
    cd Code-Commentor

### 2. Create a virtual environment

    python -m venv .venv

Activate it on Windows:

    .venv\Scripts\activate

### 3. Install dependencies

    pip install -r requirements.txt

## 🔑 API Configuration

Create a `.env` file in the project directory and add your OpenRouter API key:

    OPENROUTER_API_KEY=your_openrouter_api_key

Never upload your actual `.env` file or API key to GitHub.

## 🦙 Ollama Setup

To use Llama 3.2 locally, install Ollama and pull the model:

    ollama pull llama3.2

The project connects to the local Ollama API through:

    http://localhost:11434/v1

## 🚀 Usage

1. Open `code_commentor.ipynb`.
2. Run the notebook cells.
3. Select a model from the dropdown.
4. Enter your source code.
5. Click **Convert**.
6. The commented code will be displayed in the output box.

## 💡 Example

### Input

    def calculate(x, y):
        result = x * 2
        if result > y:
            return result - y
        return y - result

### Output

    def calculate(x, y):
        # Multiply x by 2 and store the result
        result = x * 2

        # Check if the calculated result is greater than y
        if result > y:
            # Return the difference between result and y
            return result - y

        # Return the difference between y and result
        return y - result

The original program logic is preserved. The model adds explanatory comments without changing the intended functionality.

## 🔄 How It Works

    User enters code
            ↓
    Select a model
            ↓
    Create prompts
            ↓
    Send code to the selected LLM
            ↓
    LLM analyzes the code
            ↓
    Generate comments
            ↓
    Display commented code

## 🎯 Project Goal

The goal of Code Commentor is to make source code easier to understand, especially for beginners, by automatically generating clear and meaningful comments.

## 🔮 Future Improvements

- Support more programming languages
- Add syntax highlighting
- Add code download functionality
- Add side-by-side code comparison
- Add different comment-detail levels
- Support complete project folders
- Improve generated comment accuracy


## 👨‍💻 Author

**Saif Mohammed**

GitHub:

https://github.com/saif-mohammed9505

---

## License

This project is intended for educational and experimental purposes.
