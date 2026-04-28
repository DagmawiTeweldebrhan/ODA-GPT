# ODAGPT
[![Ask DeepWiki](https://devin.ai/assets/askdeepwiki.png)](https://deepwiki.com/Hundaol-Aberra/ODA-GPT)

ODAGPT is a desktop AI chatbot designed to bridge language gaps, with a special focus on underrepresented languages from Ethiopia. It leverages real-time translation and powerful language models to enable seamless communication across different languages.

## Overview

ODAGPT allows you to interact with an AI in your native language. You type a message, the system translates it for an AI model to process, and then translates the AI's response back into your selected language. The application features a full user authentication system and persists chat history for each user.

## Features

-   **Multilingual Chat:** Supports real-time conversations in English, Amharic, Afaan Oromo, Tigrinya, and Somali.
-   **Real-time Translation:** Utilizes the Google Translate API (via `deep-translator`) to convert user input for the AI and translate the AI's response back to the user's chosen language.
-   **AI-Powered Responses:** Integrates with the Google Gemini API to provide intelligent and context-aware answers.
-   **User Authentication:** A secure login and sign-up system to manage user accounts, with credentials stored in a local SQLite database.
-   **Persistent Chat History:** Saves your conversation history to the database, which is loaded and displayed in the UI upon login for easy reference.
-   **Intuitive GUI:** Built with CustomTkinter for a modern and clean, full-screen user experience.

## Tech Stack

-   **Language:** Python
-   **GUI Framework:** CustomTkinter, Pillow
-   **AI:** Google Gemini API (`google-generativeai`)
-   **Translation:** Deep-Translator library
-   **Database:** SQLite3

## Installation and Setup

Follow these steps to get ODAGPT running on your local machine.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/hundaol-aberra/oda-gpt.git
    cd oda-gpt
    ```

2.  **Install dependencies:**
    ```bash
    pip install customtkinter Pillow google-generativeai deep-translator
    ```

3.  **Configure API Key:**
    -   Obtain a free Google Gemini API Key from [Google AI Studio](https://aistudio.google.com/app/apikey).
    -   Open the `odagpt.py` file in a text editor.
    -   Locate the `API_KEY` variable and replace the placeholder with your key:
        ```python
        API_KEY = 'YOUR_GEMINI_API_KEY_HERE' # enter your API key
        ```

## How to Use

1.  Run the application from your terminal:
    ```bash
    python odagpt.py
    ```

2.  The application will launch in fullscreen. Click the **CONTINUE** button on the welcome screen.

3.  On the login screen, either log in with existing credentials or click the **SignUp** text to create a new account.

4.  Once logged in, you will be directed to the main chat interface. Your previous chat history will be loaded on the left-hand side.

5.  Type your message in the input field at the bottom of the screen.

6.  Select your desired output language from the buttons on the right side of the screen (e.g., `A/OROMOO`, `AMHARIC`, `ENGLISH`).

7.  Press the send button or hit the `Enter` key to get a response.

8.  The conversation will appear in the main chat window. To start a new conversation, simply type a new message.

## Contributing

Contributions are welcome! If you'd like to improve ODAGPT, please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## License

This project is licensed under the MIT License.
