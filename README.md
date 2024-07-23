# Flask Chat Application with OpenAI Integration
This is a Flask-based web application that integrates OpenAI's GPT-3.5-turbo model for conversational assistance and speech-to-text capabilities. The application allows users to interact with an AI assistant, receive grades on their responses, and convert text responses to speech. The system also provides a web interface for tracking conversations and grades.

## Features
AI-Powered Chat: Engage in conversation with an AI assistant using OpenAI's GPT-3.5-turbo model.
Speech Recognition: Convert spoken input to text using Google Speech Recognition.
Text-to-Speech: Convert AI responses to speech using pyttsx3.
Real-Time Updates: Use Flask-SocketIO for real-time updates of conversations and grades.
Cloud Deployment: Deploy the application on Render for scalability.
Secure QR Code Attendance: Not implemented in this file but mentioned for context.

## Requirements
Python 3.x
Flask
Flask-SocketIO
OpenAI
SpeechRecognition
pyttsx3

## Usage

1. Navigate to the Web Interface:
   Open your web browser and go to http://localhost:5000 to access the application.

2. Interact with the AI:
   Use the microphone to provide spoken input. The AI will respond, and the response will be converted to speech.

3. View Conversations and Grades:
   The conversation and grades are updated in real-time and can be viewed on the web interface.

4. Exit the Application:
   Say "exit", "goodbye", or "leave" to end the session.

## Endpoints
GET /: Renders the main application page.
POST /process: Processes user input, generates AI responses, and updates conversations and grades.
GET /exit: Exits the application and stops the SocketIO server.
