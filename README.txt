# OpenAI Chat GUI Application #

## Overview

This Python application provides a graphical user interface (GUI) for interacting with OpenAI's Chat API. It features speech recognition, text-to-speech capabilities, and a customizable configuration for the OpenAI API. Users can interact with the OpenAI chat model using text input or voice commands, and receive spoken responses.

## Features

- **OpenAI Chat Integration**: Connects with OpenAI's Chat API to have conversations with an AI model.
- **Speech Recognition**: Converts spoken words into text using Google's Speech Recognition API.
- **Text-to-Speech**: Converts AI's textual response into speech using gTTS (Google Text-to-Speech).
- **Customizable Settings**: Allows users to configure API keys, model types, and assistant's role/name.
- **Chat Context Management**: Maintains a history of the conversation for context.
- **Audio Playback Control**: Ability to stop ongoing speech playback.
- **GUI Interface**: Easy-to-use interface built with Tkinter.

## Prerequisites

- Python 3.x
- OpenAI API Key
- Internet connection for speech services and OpenAI API

## Installation

1. Clone the repository or download the source code.
2. Install the required dependencies:
   ```bash
   pip install openai gtts pygame speech_recognition
   ```

## Usage

1. Run the script:
   ```bash
   python3 main.py
   ```
2. Enter your OpenAI API key and other configurations in the settings dialog.
3. Use the GUI to type or speak your messages.
4. The AI's responses will be displayed in text and spoken out loud.

## Configuration

- **API Key**: Your personal OpenAI API key.
- **Model**: The specific model of OpenAI to use (e.g., `text-davinci-003`).
- **Assistant's Role**: Role identifier for the assistant (e.g., `assistant`).
- **Assistant's Name**: Custom name for your assistant.

## Voice Commands

- Use the "Voice Input" button to start speech recognition.
- Speak clearly into your microphone.
- Your spoken words will be converted to text and sent to the OpenAI model.

## Controls

- **Send**: Send the typed message to the OpenAI model.
- **Voice Input**: Start voice command recognition.
- **Stop Speech**: Immediately stop any ongoing speech playback.
- **Clear**: Clear the chat history.

## Troubleshooting

- Ensure your API key is valid and has the necessary permissions.
- Check your internet connection for speech and API services.
- For speech recognition issues, ensure your microphone is properly configured.

## License

This project is licensed under the Apache 2.0 License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for the API.
- Google's gTTS and Speech Recognition for speech services.
- Pygame for audio handling.

---

End of README. This guide provides all the necessary information for getting started with the application, including installation, usage, configuration, and troubleshooting.
