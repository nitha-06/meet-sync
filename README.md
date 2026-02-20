An AI-powered Google Calendar assistant built with n8n, LangChain Agent, and OpenAI (gpt-5-mini).

This workflow allows users to interact with Google Calendar using natural language via chat.

🚀 Features

💬 Chat-based trigger

🤖 AI Agent powered by OpenAI

📅 Fetches multiple events from Google Calendar

🔗 Tool-based agent integration

🧠 Natural language understanding for calendar queries

🏗 Workflow Architecture
Chat Trigger
     ↓
AI Agent (LangChain)
     ↓
OpenAI Chat Model (gpt-5-mini)
     ↓
Google Calendar Tool (Get Many Events)
📦 Requirements

n8n (latest version recommended)

OpenAI API Key

Google Calendar OAuth2 Credentials

Google Calendar API enabled in Google Cloud Console

⚙️ Setup Instructions
1️⃣ Import Workflow

Copy the provided JSON workflow file

In n8n → Import → Paste JSON

2️⃣ Configure Credentials

You must manually configure:

OpenAI API credentials

Google Calendar OAuth2 credentials

Attach them to:

OpenAI Chat Model

Get many events in Google Calendar

3️⃣ Select Calendar

Inside the Google Calendar node:

Choose the desired calendar

Ensure proper read permissions

4️⃣ Activate Workflow

Toggle the workflow to Active

💬 Example Prompts

You can ask:

“What meetings do I have tomorrow?”

“List my events this week.”

“Do I have anything scheduled on Friday?”

“Show all upcoming events.”

🔒 Security Notes

Credentials are NOT included in this repository.

Never commit API keys.

Use environment variables where possible.

🛠 Customization Ideas

You can extend this workflow by adding:

Create event tool

Update event tool

Delete event tool

Availability checking

Smart scheduling logic

Slack or WhatsApp integration

📄 Workflow Metadata

Agent Type: LangChain Agent

Model: gpt-5-mini

Calendar Operation: getAll

Execution Mode: v1
