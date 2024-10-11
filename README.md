def chatbot_response(user_input):
    user_input = user_input.lower()  # Convert input to lowercase for case-insensitive matching

    if "hey chatbot" in user_input or "hi" in user_input or "hello" in user_input:
        return "Hello! How can I help you today?"
    elif "how are you" in user_input:
        return "I'm just a chatbot, but I'm here to help! How can I assist you?"
    elif "what is your name" in user_input:
        return "you can call me ChatBot!"
    elif "goodbye" in user_input or "bye" in user_input:
        return "Goodbye! Have a great day!"
    elif "thank you" in user_input:
        return "You're welcome! Feel free to ask if you need more help."
    elif "weather" in user_input:
        return "I can't predict the weather. You can take the help of google."
    else:
        return "I'm not sure how to respond to that. Can you please rephrase or ask something else?"

# Example usage
while True:
    user_input = input("You: ")
    if user_input.lower() == "exit":
        break
    response = chatbot_response(user_input)
    print("ChatBot:", response)