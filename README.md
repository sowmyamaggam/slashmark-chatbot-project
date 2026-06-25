# slashmark-chatbot-project
# Advanced Simple AI Chatbot

print("=== AI CHATBOT ===")
print("Type 'bye' to exit.\n")

while True:
    user = input("You: ").lower()

    # Greetings
    if user in ["hi", "hello", "hey"]:
        print("Bot: Hello! Nice to meet you.")

    # How are you
    elif "how are you" in user:
        print("Bot: I am doing great! What about you?")

    # Name
    elif "your name" in user:
        print("Bot: I am your Python chatbot.")

    # Time
    elif "time" in user:
        from datetime import datetime
        current_time = datetime.now().strftime("%H:%M:%S")
        print("Bot: Current time is", current_time)

    # Date
    elif "date" in user:
        from datetime import date
        today = date.today()
        print("Bot: Today's date is", today)

    # Help
    elif "help" in user:
        print("Bot: You can ask me about time, date, greetings, or simple questions.")

    # Feeling
    elif "fine" in user or "good" in user:
        print("Bot: That's great to hear!")

    elif "sad" in user:
        print("Bot: Don't worry. Everything will be okay.")

    # Study
    elif "study" in user:
        print("Bot: Study regularly and practice coding daily.")

    # Favourite color
    elif "favorite color" in user or "favourite color" in user:
        print("Bot: I like blue color.")

    # Creator
    elif "who created you" in user:
        print("Bot: I was created using Python.")

    # Joke
    elif "joke" in user:
        print("Bot: Why do programmers love Python? Because it's easy to understand!")

    # Bye
    elif user == "bye":
        print("Bot: Goodbye! Have a nice day.")
        break

    # Default response
    else:
        print("Bot: Sorry, I don't understand that yet.")
