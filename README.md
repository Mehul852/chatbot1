
# Chatbot

## What are chatbots?

A chatbot is an artificial intelligence (AI) software designed to simulate human conversation through text or voice interactions.


## About project.

This project involves creating a simple interactive application that combines user data collection with a conversational AI model.

## Project Components

1.Data base setup
* Purpose: To store user details persistently.
* Database: SQLite, a lightweight, disk-based database that is easy to set up and use.
* Table Structure:
  * id: Integer, primary key, auto-incremented.
  * name: Text, user's name.
  * mobile_number: Text, user's mobile number.
  * email_id: Text, user's email ID.
  * date_of_birth: Text, user's date of birth.

2.User interaction 
* Collecting Data: Using Python's input function to collect user details such as name, mobile number, email ID, and date of birth.
* Storing Data: Inserting the collected data into the SQLite database.
3.Coversational AI
* Model: DialoGPT, provided by Hugging Face's transformers library.
* Functionality: Using the model to generate conversational responses based on user input.
* Interaction: A loop that continues to prompt the user for input and generate responses until the user types 'ok' to end the conversation.

## Code overview 

1. Database Creation
* Connects to an SQLite database and creates a table if it doesn't already exist.
2. Gathering User Details
* Prompts the user to enter their details and stores these details in the database.
3. Setting Up the Conversational AI Model
* Loads the pre-trained DialoGPT model and tokenizer from the Hugging Face library.
4. Generating Responses
* Encodes user input, updates the chat history, generates a response using the model, and decodes the response into readable text.
5. Main Program Loop
* Continuously prompts the user for input, generates responses, and prints them until the user types 'ok' to end the conversation.

## Potential Applications

1. Customer Service
2. Educational Tools
3. Personal Assistants

## Summary

This project demonstrates a basic yet functional integration of user data collection with a conversational AI model. It serves as a foundational example of how to build more complex applications that involve database management and natural language processing.


