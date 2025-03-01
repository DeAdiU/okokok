# Chat AI API

A backend API for interacting with an AI-powered chatbot, built using Django REST Framework (DRF). The application allows users to register, log in, and send messages to the AI, which provides responses. Tokens are deducted for each interaction, and the chat history is recorded.

## Features

- User registration and authentication (JWT-based).
- Send messages to the AI chatbot and receive responses.
- Token management, with deduction for each query.
- Chat history tracking, including user messages and AI responses.
- API documentation via Swagger.

## Requirements

- Python 3.12+
- Django 4.x
- Django REST Framework
- PyJWT
- Google Generative AI (Gemini) SDK

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YourUsername/Chat-AI-API.git
   cd Chat-AI-API

2. Create a virtual environment and install dependencies:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt

3. Apply migrations and run the server:
    ```bash 
    python manage.py makemigrations
    python manage.py migrate
    python manage.py runserver

## API Endpoints

1. Authentication:
    - Login - `/login`/ (POST)
    - Register - `/register`/ (POST)
2. Chat Management:
    - Send Message - `/chat/` (POST)
3. Token Management:
    - Check Token Balance - `/tokens/balance/` (GET)
4. API Documentation:
    - Swagger API Docs - `/swagger/` 

## API Documenatation

The project has integrated Swagger for easy API documentation. You can access the Swagger UI by navigating to the /swagger/ URL when the server is running. Please use the Authorize button to enter your JWT token for accessing protected routes.
    
## Contributing

Contributions are welcome! Please fork the repository and create a pull request to submit changes.
