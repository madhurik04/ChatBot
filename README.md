# Chatbot Using PyTorch

## Overview

This project implements a simple FAQ chatbot using PyTorch for natural language processing (NLP). The chatbot is designed to answer frequently asked questions (FAQs) by matching user queries to predefined answers using a machine learning model.

## Features

- **Natural Language Understanding**: Utilizes NLP techniques to understand and respond to user queries.
- **Predefined FAQ Matching**: Matches user questions to a set of predefined FAQs to provide relevant answers.
- **Easy Deployment**: Built using Flask, making it easy to deploy as a web service.

## Prerequisites

- Python 3.6 or newer
- Pip (Python package installer)

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/madhurik04/ChatBot.git
    cd ChatBot.git
    ```

2. **Create a Virtual Environment** (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install the Required Packages**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Download SpaCy Model**:
    ```bash
    python -m spacy download en_core_web_sm
    ```

## Running the Chatbot

1. **Start the Flask Application**:
    ```bash
    python chatbot.py
    ```

2. **Access the Chatbot**:
    - Open your browser and navigate to `http://127.0.0.1:5000`
    - Alternatively, you can use a tool like Postman to interact with the chatbot via its API.

### Using curl

To test the chatbot, you can send a POST request using curl:

```bash
curl -X POST http://127.0.0.1:5000/chatbot -H "Content-Type: application/json" -d "{\"question\": \"What are your opening hours?\"}"
