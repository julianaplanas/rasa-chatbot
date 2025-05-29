# Birthday Message Bot

## Overview
This project is a conversational bot designed to help users write a happy birthday message to a friend or family member. The bot interacts with users to collect the recipient's name and the date of their birthday and then generates a birthday message.

## Features
- Collects the recipient's name.
- Collects the date of the recipient's birthday.
- Generates a personalized happy birthday message.

## How to Use

### 1. Install Dependencies
Ensure you have Python 3.11 installed. Create a virtual environment and install the required dependencies:
```bash
python3.11 -m venv venv
source venv/bin/activate
pip install rasa-pro
```

### 2. Train the Bot
Train the bot using Rasa:
```bash
rasa train
```

### 3. Run the Bot
Start the Rasa server:
```bash
rasa inspect
```

## Project Structure
- **`config.yml`**: Configuration for the bot's pipeline and policies.
- **`domain.yml`**: Defines intents, slots, responses, and actions.
- **`data/flows.yml`**: Contains the conversational flow for writing a birthday message.
- **`actions/actions.py`**: Custom actions for generating the birthday message.

## Example Interaction
1. The bot asks: "What is the name of the person you'd like to send a birthday message to?"
2. The user provides the name.
3. The bot asks: "What is the date of their birthday?"
4. The user provides the date.
5. The bot responds: "Happy Birthday, [Name]! 🎉 Have a wonderful day!"

Enjoy using the Birthday Message Bot!