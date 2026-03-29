# 🤖 AI Telegram Assistant for E-Commerce

An automated AI-driven customer support assistant built using n8n.  
This project connects a Telegram bot with Google Gemini AI to provide intelligent, context-aware responses to customer inquiries about products and services.


## 🚀 Overview

The assistant acts as a first-line support agent, handling customer questions in real time.

### Example Use Case
The bot can:
- Respond to product inquiries (e.g., traditional Ukrainian clothing — *Vyshyvanka*)
- Provide:
  - Product descriptions
  - Pricing
  - Purchase links
- Offer additional help (e.g., choosing the right size)


## 🧠 Workflow Visualization

Below is a visual representation of the workflow in n8n:

![Workflow Screenshot](https://github.com/Khadjiitka/n8n_AI_Agent_vyshivanki/blob/03ce46398fe48783794c2b5f943711c2baeb4add/n8n.png)


## 🛠 Features

- ⚡️ Real-time Interaction  
  Uses a Telegram Trigger node to instantly receive incoming messages.

- 🤖 Intelligent Reasoning  
  Powered by Google Gemini for natural language understanding and response generation.

- 🧩 Memory Management  
  Maintains conversation context using a Simple Memory node.

- 📩 Automated Responses  
  Sends replies back to users via Telegram automatically.

## 📋 System Architecture

The workflow consists of three main components:

### 1. Telegram Trigger
- Listens for incoming user messages
- Acts as the entry point of the workflow

### 2. AI Agent Node
- Core logic of the assistant
- Processes incoming messages using:
  - Model: Google Gemini
  - Memory: Stores conversation context for follow-ups

### 3. Telegram Send Message
- Sends the generated AI response back to the user
