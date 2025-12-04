# Agent Development Kit (ADK) - Agent Observability - Logs, Traces & Metrics

In this codelab, you'll learn: How to add observability to the agent you've built and how to evaluate if the agents are working as expected

## Getting Started

### Setup Environment

Follow these steps to set it up:

```bash
# Create virtual environment in the root directory
uv venv

# Activate
# macOS/Linux:
source .venv/bin/activate
# Windows CMD:
.venv\Scripts\activate.bat
# Windows PowerShell:
.venv\Scripts\Activate.ps1

# Install dependencies
uv sync
```

### Setting Up API Keys

1. Create an account in Google Cloud https://cloud.google.com/?hl=en
2. Create a new project
3. Go to https://aistudio.google.com/apikey
4. Create an API key
5. Assign key to the project

The agent folder contains a `.env.example` file:

1. Navigate to the agent folder
2. Rename `.env.example` to `.env` 
3. Open the `.env` file and replace the placeholder with your API key:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```