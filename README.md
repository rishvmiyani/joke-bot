#Joke Bot Setup Instructions

This guide will help you set up and run the Joke Bot using Telegram and OpenAI on your local machine (Linux/Termux/Windows with Python installed).


---

Prerequisites

Python 3.10 or above

A Telegram Bot Token from BotFather

An OpenAI API key from https://platform.openai.com/account/api-keys

Git & pip installed



---

1. Clone the Repository

git clone https://github.com/rishvmiyani/joke-bot.git
cd joke-bot


---

2. Create .env File

Create a .env file in the project root:

TELEGRAM_BOT_TOKEN=your-telegram-bot-token-here
OPENAI_API_KEY=your-openai-api-key-here

> Tip: You can copy from .env.example and update your keys.




---

3. Install Dependencies

First, upgrade pip:

pip install --upgrade pip setuptools wheel

Then install all required packages:

pip install -r requirements.txt

> If you're on Termux and face issues with OpenAI install, use:



pip install "openai>=1.0.0,<2.0.0"


---

4. Run the Bot

Simply start the bot using:

python assistant.py

You should see:

Bot is running...

Go to Telegram and type /joke to your bot. It should reply with a short funny joke.


---

5. Troubleshooting

ModuleNotFoundError: Run pip install -r requirements.txt again.

Bot not responding: Check if your bot token is correct and bot is not blocked.

OpenAI error: Ensure your OpenAI key is correct and has usage access.



---

