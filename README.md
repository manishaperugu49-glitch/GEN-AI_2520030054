# LLM Starter – Google Gemini API with Python

## 📌 Project Overview

This project demonstrates how to connect Python with Google's Gemini API using the Google AI Studio API key.

It sends a text prompt to the Gemini model and displays the AI-generated response in the terminal.

## 🚀 Features

- Connects Python with Google Gemini API.
- Uses Google AI Studio API key for authentication.
- Sends text prompts to the Gemini model.
- Receives and displays AI-generated responses.
- Includes basic error handling and retry functionality.

## 🛠️ Technologies Used

- Python
- Google Gemini API
- Google Gen AI Python SDK
- VS Code
- PowerShell
- Python Virtual Environment (`venv`)

## 📂 Project Structure

```text
llm-starter/
│
├── .venv/
├── hello_llm.py
├── README.md
└── .gitignore
```

## ⚙️ Installation and Setup

### 1. Clone or open the project

```powershell
cd C:\llm-starter
```

### 2. Create a virtual environment

```powershell
python -m venv .venv
```

### 3. Activate the virtual environment

```powershell
.\.venv\Scripts\Activate.ps1
```

### 4. Install the Google Gen AI SDK

```powershell
pip install google-genai
```

### 5. Get your Google AI Studio API Key

1. Visit https://aistudio.google.com/apikey
2. Sign in using your Google account.
3. Create an API key.
4. Copy your API key.

### 6. Configure the API key

In PowerShell, execute:

```powershell
$env:GEMINI_API_KEY="YOUR_API_KEY"
```

Replace `YOUR_API_KEY` with your actual API key.

**Note:** This environment variable is available only in the current PowerShell session.

## ▶️ Running the Project

Execute the following command:

```powershell
python hello_llm.py
```

The program sends a prompt to Gemini:

```text
Hello! Introduce yourself.
```

Gemini generates a response, which is displayed in the terminal.

## 🔐 Security

- Never upload your API key to GitHub.
- Never share your API key publicly.
- Use environment variables to store API credentials.
- Add `.env` and other secret files to `.gitignore` if you use them.

## ⚠️ Error Handling

The application includes basic retry handling.

Common errors:

| Error | Possible Reason |
|---|---|
| API key not found | Environment variable is missing |
| 401 Unauthorized | Invalid API key |
| 403 Forbidden | API access or permission issue |
| 429 Too Many Requests | Rate limit exceeded |
| 503 Service Unavailable | Temporary server overload |

## 🎯 Expected Output

```text
Connecting to Gemini...

Gemini Response:

Hello! I'm Gemini, an AI assistant...
```

*The actual response depends on the Gemini model.*

## 📚 Learning Outcomes

After completing this project, you will understand:

- How to connect Python applications to an LLM.
- How to authenticate using an API key.
- How to send prompts to a Generative AI model.
- How to receive AI-generated responses.
- How to handle API errors.

## 👩‍💻 Author

Manisha Perugu

## 📄 License

This project is created for educational and learning purposes.
