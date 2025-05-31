# HotelBookingBot – AI Chatbot with Amazon Lex

HotelBookingBot is an intelligent conversational assistant built using **Amazon Lex** and **AWS Lambda**, designed to help users book, cancel, or modify hotel reservations via natural language.

---

## Features

- Book a hotel room with customizable options
- Greet users with friendly messages
- Fallback intent for unrecognized queries

---
## Architecture

User ➝ Amazon Lex ➝ AWS Lambda 

- **Amazon Lex**: Handles natural language processing and intents
- **AWS Lambda**: Fulfillment logic for all chatbot intents

How to Deploy
Step 1: Create the Chatbot in Amazon Lex
Create HotelBookingBot

Add intents: BookHotel, Greeting, FallbackIntent

Define sample utterances and required slots

Step 2: Create and Link Lambda Function
Go to AWS Lambda → Create Function → Name: HotelBookingLambda

Runtime: Python 3.9

Paste logic from lambda_function.py

Attach Lex permissions

Link the Lambda function to each intent under Fulfillment

Step 3: Build and Test
Click "Build" in Lex

Open Test Bot window and try:

"Hi"
"Book a hotel"




