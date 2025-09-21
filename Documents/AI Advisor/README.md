# Career-AI-Advisory

Small repo with an AI Learning Path advisor built with Azure OpenAI and Gradio.

## Quick start

1. Create a Python virtual environment and install requirements:

`powershell
python -m venv .venv
.\.venv\Scripts\activate.bat  # or use the preferred activation method below
pip install -r requirements.txt
`

2. Create a local .env file. Copy the variables from .env.example and fill in your real API key and endpoint:

`
AZURE_OPENAI_API_KEY=your_real_key_here
AZURE_OPENAI_ENDPOINT=https://your-resource.openai.azure.com/
AZURE_OPENAI_DEPLOYMENT=gpt-4o
`

3. Run the app (example):

`powershell
python "Class-1\AI Foundry\foundry_chat_bot.py"
`

## Activation option for PowerShell

`powershell
.\.venv\Scripts\activate.bat
`
