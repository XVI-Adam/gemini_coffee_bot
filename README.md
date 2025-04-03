# Coffee Shop Chatbot with Gemini and Taipy

This repository contains code for a coffee shop chatbot built using Google's Gemini 1.5 Flash model and the Taipy GUI framework. The chatbot is designed to take coffee orders based on a specific menu and follow a predefined set of conversational rules.

## Prerequisites

Before running the application, ensure you have the following installed:

-   Python 3.6 or later
-   `pip` (Python package installer)
-   Google's `genai` library
-   `python-dotenv` library
-   `taipy` library

You can install the required packages using pip:

```bash
pip install google-generativeai python-dotenv taipy

## Key Features

-   **Gemini Integration:** Uses Google's Gemini 1.5 Flash to handle coffee order conversations.
-   **Taipy GUI:** Provides a simple web interface for user interaction.
-   **JSON Response Handling:** Parses Gemini's JSON output for structured responses.
-   **Contextual Conversations:** Manages order flow based on system instructions.
-   **Menu-Based Ordering:** Restricts orders to a predefined menu.
-   **.env API Key Management:** Securely loads API key from a `.env` file.

## Core Code Functionality

-   **`user_replied(state, var_name, value)`:** Sends user input to Gemini and updates the chatbot's response.
-   **`extract_json(s)`:** Extracts JSON from Gemini's text output.
-   **`chat_config`:** Configures Gemini with system instructions for order handling.
-   **`Gui(page).run(...)`:** Launches the Taipy GUI.
