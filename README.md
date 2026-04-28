ODAGPT

ODAGPT is a local-language AI chatbot that breaks communication barriers using real-time translation and AI-generated responses. It focuses on accessibility and support for underrepresented languages.

Overview

ODAGPT lets you interact in your native language while the system handles translation and response generation.

You type in one language. The system translates it, processes it using AI, and returns a response in your selected language.

Features
Multilingual Support
Communicate across different languages in real time
Text-Based Interaction
Input and output are currently text only
AI-Powered Responses
Uses Gemini API for generating responses
Real-Time Translation
Integrated with Google Translate API
Custom UI
Built using customtkinter
Accessibility-Oriented Design
Focused on simplifying communication across language barriers

System Architecture
User Input (Text)
        ↓
Language Detection
        ↓
Translation (to processing language)
        ↓
AI Processing (Gemini API)
        ↓
Translation (to target language)
        ↓
Output (Text)

Tech Stack

Language: Python
UI: customtkinter
AI Model: Gemini API
Translation: Google Translate API

Installation

Clone the repository
git clone https://github.com/your-username/odagpt.git
cd odagpt

Set up API keys

Create a .env file:

GEMINI_API_KEY=your_key_here
GOOGLE_TRANSLATE_API_KEY=your_key_here

Run the application
python main.py

Usage
Launch the app
Select input and output languages
Enter text
View translated AI response

Project Goals

Support Ethiopian and other low-resource languages
Work in low-bandwidth environments
Provide a simple AI interface for multilingual communication

Limitations

Text-only interaction, no speech features yet
Depends on internet connection for APIs
Translation accuracy varies by language

Future Improvements

Add speech-to-text and text-to-speech
Offline-first functionality
Custom-trained models for local languages
Mobile version

Contributing
Fork the repository
Create a branch
Submit a pull request

License

MIT License
