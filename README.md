# telegram-bot-moderator
Telegram bot that automatically deletes messages with undesirable words in groups and notifies the chat with censored versions. Replies with functionality info in private messages.

## Telegram Censor Bot

A Telegram bot that automatically deletes messages containing undesirable words in groups and notifies the chat with censored versions of the words.  
In private messages, the bot explains its functionality.

---

## Features

- **Private chats**: Replies with an explanation of its functionality.
- **Group chats**: 
  - Deletes messages containing trigger words.
  - Sends a notification showing which words were removed, with all characters except the first and last replaced by `*` (censored).
- **Trigger words** are stored in `trigger.txt` and can be customized.
- **Token** is stored separately in `token.txt` for security.

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/USERNAME/telegram-censor-bot.git
cd telegram-censor-bot

2. Create a file named token.txt in the repository folder and paste your bot token:
1234567890:ABCdefGhIJKlmNoPQRstuVWXyz123456789

3. Edit trigger.txt to add words that should be deleted (one per line).

4. Install the required library:
pip install pyTelegramBotAPI

5. Run the bot:
python bot.py
