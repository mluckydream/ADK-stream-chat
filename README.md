# ADK Streaming Chat 

## Overview

This project demonstrates a real-time chat application that uses the Google ADK (AI Development Kit) to interact with a Large Language Model (LLM) and perform searches using the `google_search` tool. The application is built using FastAPI for the backend and HTML/CSS for the frontend.
It allows users to send messages to the chatbot, which responds using information fetched from Google Search.

## Features

- **Real-time Chat**: Users can send messages to the chatbot in real-time.
- **Google Search Integration**: The chatbot can perform searches using the `google_search` tool to provide accurate and up-to-date information.
- **WebSocket Communication**: The frontend communicates with the backend using WebSockets for real-time updates.

## Prerequisites

- Python 3.8 or higher
- Google ADK SDK
- FastAPI
- Uvicorn (ASGI server for FastAPI)

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/mluckydream/ADK-stream-chat.git
cd adk-streaming-test
```
2. Install Dependencies
Create a virtual environment and install the required Python packages:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
```
3. Set Environment Variables
Create a .env file in the root directory and add your Google ADK API key:

```
GOOGLE_ADK_API_KEY=your_google_adk_api_key_here
```
4. Run the Application
Start the FastAPI server using Uvicorn:

```bash
uvicorn main:app --reload
```
The application will be available at http://127.0.0.1:8000.

Project Structure
```
├── .env
├── .gitignore
├── main.py
├── requirements.txt
├── static/
│   └── index.html
└── README.md
```

### Open the Application
Navigate to http://127.0.0.1:8000 in your web browser.
Send Messages: Type a message in the input field and click "Send".
Receive Responses: The chatbot will respond using information fetched from Google Search.
Customization
Frontend

### Backend
You can extend the functionality of the chatbot by adding more tools or modifying the existing ones in the main.py file.

### Contributing
Contributions are welcome! Please open an issue or submit a pull request with your changes.

