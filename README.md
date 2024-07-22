# 🤖 Advanced Chatbot with NLTK

Welcome to the **Advanced Chatbot** project! This chatbot uses NLTK for natural language processing to provide an interactive experience. 🗣️

## 📦 Installation

To get started, you'll need to install the required Python libraries. Follow the instructions below:

1. **Open Command Prompt or Terminal**:
   - On **Windows**, you can open Command Prompt.

2. **Install NLTK**:
   Run the following command to install the NLTK library:
   ```sh
   pip install nltk

Download NLTK Data:

Open a Python shell or create a Python script and run the following code to download the necessary NLTK data files:
python

import nltk

nltk.download('punkt')

📝 Create a Python Script

Save the following code into a Python file (e.g., chatbot.py):


import random

import nltk

from nltk.tokenize import word_tokenize


# Download NLTK data (only need to run this once)

nltk.download('punkt')

def advanced_chatbot():
    print("Hello! I'm an advanced chatbot using NLTK. How can I assist you today?")

    while True:
        user_input = input("You: ").lower()
        tokens = word_tokenize(user_input)

        if any(greet in tokens for greet in ["hi", "hello", "hey"]):
            print("Bot: Hello! How can I help you today?")

        elif any(phrase in user_input for phrase in ["how are you", "how's it going", "how are you doing"]):
            print("Bot: I'm just a bot, but I'm here to help you!")

        elif "weather" in tokens:
            print("Bot: I can't check the weather right now, but you can check a weather website for that information.")

        elif "time" in tokens:
            print("Bot: I don't have a clock, but you can check the time on your device.")

        elif "name" in tokens:
            print("Bot: I'm just a simple chatbot with no name.")

        elif "joke" in tokens:
            jokes = [
                "Why don't scientists trust atoms? Because they make up everything!",
                "Why did the scarecrow win an award? Because he was outstanding in his field!",
                "Why don't programmers like nature? It has too many bugs."
            ]
            print(f"Bot: {random.choice(jokes)}")

        elif "bye" in tokens or "exit" in tokens:
            print("Bot: Goodbye! Have a great day!")
            break

        else:
            print("Bot: I'm not sure how to respond to that. Can you ask something else?")

# Run the advanced chatbot function

advanced_chatbot()

🚀 Run the Script

Navigate to the directory where you saved chatbot.py and run the script using Python

