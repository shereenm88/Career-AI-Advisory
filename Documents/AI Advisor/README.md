# Career-AI-Advisory

Small repo with an AI Learning Path advisor built with Azure OpenAI and Gradio.

## Quick start

1. Create a Python virtual environment and install requirements:

`powershell
python -m venv .venv
.\.venv\Scripts\activate.bat  # or use the preferred activation method below
pip install -r requirements.txt
`

2. Create a local .env file (do NOT commit this file). Copy the variables from .env.example and fill in your real API key and endpoint:

`
AZURE_OPENAI_API_KEY=your_real_key_here
AZURE_OPENAI_ENDPOINT=https://your-resource.openai.azure.com/
AZURE_OPENAI_DEPLOYMENT=gpt-4o
`

3. Run the app (example):

`powershell
python "Class-1\AI Foundry\foundry_chat_bot.py"
`

## Activation options for PowerShell

- Use the batch script (no policy change):

`powershell
.\.venv\Scripts\activate.bat
`

- One-off bypass (temporary, safe for single command):

`powershell
PowerShell -ExecutionPolicy Bypass -NoProfile -Command ". .\.venv\Scripts\Activate.ps1"
`

- Persist for your user (RemoteSigned):

`powershell
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned -Force
`

## Security notes

- Never commit .env or real API keys. This repo includes .env.example as a template and .gitignore excludes .env and .venv.
- If an API key is ever exposed, rotate it immediately in the Azure portal.
- For CI, store secrets in GitHub Actions secrets and reference them as ${{ secrets.AZURE_OPENAI_API_KEY }}.

## Files of interest

- Class-1/AI Foundry/foundry_chat_bot.py  the Gradio chat app and prompt setup.
- .env.example  example environment variables (no secrets).

