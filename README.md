🤖 Telegram AI Agent using n8n

This project is an AI-powered Telegram bot built using n8n, OpenAI, and LangChain agent tools.
It can respond to user text, convert voice messages to text, use memory, and even perform live internet searches using LangSearch.

🚀 Features :

✅ 1. Telegram Chatbot (Two-way Messaging)

Receives messages using Telegram Trigger Node

Sends replies back using Telegram Send Message Node

✅ 2. AI Agent with System Rules

The bot is set up as Leo Bot (Leo Das) — an intelligent assistant with:

Greeting rules

Polite responses

Smart handling of prompts

Internet search tool access

🧠 3. Memory Support :

Stores previous messages for each user using:

Memory Buffer Window node
This allows more natural conversations.

🎤 4. Voice Message Support :

Detects voice messages

Downloads audio file

Transcribes using OpenAI Whisper

🌐 5. Internet Search Tool :

Uses an HTTP Request Tool to search online via LangSearch API.

🤖 6. OpenAI Chat Model Integration :

Uses gpt-4.1-nano for generating intelligent responses.

🏗️ Workflow Structure :

| Node                     | Purpose                            |
| ------------------------ | ---------------------------------- |
| **Telegram Trigger**     | Receives messages from Telegram    |
| **Switch Node**          | Checks if message is text or voice |
| **AI Agent (LangChain)** | Core brain of the bot              |
| **OpenAI Chat Model**    | LLM used for generating replies    |
| **Memory Buffer**        | Maintains conversation memory      |
| **Transcription Node**   | Converts voice → text              |
| **HTTP Request Tool**    | Allows internet search queries     |
| **Send Message Node**    | Sends responses back to user       |




⚙️ How to Use This Workflow


1️⃣ Import Workflow into n8n

Go to n8n → Workflows → Import from File

Select First Telegram Bot.json

2️⃣ Add Your Credentials

You need:

OpenAI API key

Telegram Bot Token

LangSearch API key

3️⃣ Activate Workflow

Click Activate and start chatting with your bot in Telegram.
