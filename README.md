# AI-food-ordering-agent
AI Food Ordering Assistant (n8n)

An AI-powered food ordering assistant built using n8n and Google Gemini, capable of handling customer conversations, checking inventory, answering FAQs, and storing orders in real-time using Google Sheets.

Features
Conversational AI chatbot for food ordering
Real-time inventory checking
Automatic order storage in Google Sheets
FAQ handling (delivery time, payment, etc.)
Context-aware conversation using memory
Order validation (available / out of stock)
Workflow Overview

This project uses an AI Agent inside n8n to automate the food ordering process:

Trigger

Starts when a user sends a chat message

AI Agent

Processes user intent (order, FAQ, stock check)
Guides user step-by-step (name → item → quantity)

Memory

Maintains conversation context for better interaction

Integrated Tools (Google Sheets)
Inventory Sheet → Check available food items
FAQ Sheet → Answer common queries
Orders Sheet → Store confirmed/rejected orders
Example Interaction

User: Hi
Bot: Welcome to Foodie Hub
How can I help you today?

User: I want 2 pizzas
Bot: Please provide your name

User: Aditi
Bot: Your order for Pizza (2) is confirmed

Tech Stack
Automation: n8n
AI Model: Google Gemini
Database: Google Sheets
Memory Handling: n8n Simple Memory
Google Sheets Structure
Inventory Sheet
Food Item	Quantity
Pizza	10
Burger	5
Orders Sheet
Customer Name	Food Item	Quantity	Order Date	Status	Description
FAQ Sheet
Question	Answer
Delivery time?	30 mins
Setup Instructions
Install n8n
Import the workflow JSON file
Connect your Google Sheets credentials
Replace Sheet IDs with your own
Connect Google Gemini API
Activate the workflow
How It Works
User sends a message
AI understands intent
Checks inventory (if needed)
Confirms or rejects order
Stores result in Google Sheets
Future Improvements
Payment integration
WhatsApp / Telegram bot integration
Admin dashboard for order tracking
Unique Order ID generation
License

This project is for learning and demonstration purposes.

Author

Aditi Verma
