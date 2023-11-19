# OpenAI Chat GUI Application #

## Overview

This Python application, `API_GUI_Chat.py`, provides a graphical user interface (GUI) for interacting with OpenAI's Chat API. It features speech recognition, text-to-speech capabilities, and customizable configurations, allowing users to converse with an AI model through text or voice commands.

## Features

- **OpenAI Chat Integration**: Facilitates conversations with OpenAI's Chat API.
- **Speech Recognition**: Converts spoken words into text using Google's Speech Recognition API.
- **Text-to-Speech**: Translates AI text responses into speech using gTTS (Google Text-to-Speech).
- **Customizable Settings**: Configurable API keys, model types, assistant's roles, and names.
- **Chat Context Management**: Maintains a conversation history for context.
- **Audio Playback Control**: Stops ongoing speech playback.
- **GUI Interface**: User-friendly interface designed with Tkinter.

## Prerequisites

- Python 3.x
- OpenAI API Key
- Internet connection for speech services and OpenAI API

## Installation

### On Windows

   **Clone the repository**:
   - Open Command Prompt and navigate to the desired directory.
   - Run `git clone https://github.com/B-Boone/OpenAI_Chat_API_GUI.git`
   - If git is not installed, download and install it from [git-scm.com](https://git-scm.com/).

   OR

   **Download Source Code**:
   - Visit `https://github.com/B-Boone/OpenAI_Chat_API_GUI`.
   - Click on 'Code' and select 'Download ZIP'.
   - Extract the ZIP file to the desired location.

### On Linux

   **Clone the repository**:
   - Open a terminal and navigate to the desired directory.
   - Run `git clone https://github.com/B-Boone/OpenAI_Chat_API_GUI.git`
   - If git is not installed, install it using your distribution's package manager.

   OR

   **Download Source Code**:
   - Visit `https://github.com/B-Boone/OpenAI_Chat_API_GUI`.
   - Click on 'Code' and select 'Download ZIP'.
   - Use `unzip <file_name>.zip` in the terminal to extract files.

### Install Dependencies

Run the following command in your terminal or command prompt:
```bash
pip install openai gtts pygame speechrecognition
```

## Usage

### Locating and Running the Script

  **Windows**:
  - Navigate to the cloned/downloaded folder.
  - Open Command Prompt here and run:
    ```bash
    python API_GUI_Chat.py
    ```

  **Linux**:
  - Open a terminal and navigate to the cloned/downloaded directory.
  - Run:
    ```bash
    python3 API_GUI_Chat.py
    ```

### Configuration

  **API Key**: Input your OpenAI API key in the provided field.
  **Model**: Choose a model from OpenAI. Compatible models include `gpt-4-1106-preview`, `gpt-4`, `gpt-4-32k`, `gpt-3.5-turbo-1106`, `gpt-3.5-turbo-instruct`
  **Assistant's Role and Name**: Customize the role and name of the AI assistant.

#### Modifying JSON Output Directories

- The default directory for audio and context JSON files is set to `os.path.join(os.environ['APPDATA'], 'API_GUI_Chat')` for Windows.
- To change this directory, modify `audio_dir` and `context_file` paths for the `speak` and `load_chat_context`/`save_chat_context` functions.

- The default directory for the settings config JSON file is set to the path of the python file.
- To change thes directory, modify `save_configuration` and `load_configuration` filenames.

#### Changing Context Limit

- Locate the `send_message_original` function.
- Modify `if len(chat_context) > 10:` and `chat_context = chat_context[-10:]` to your desired context size.

## Voice Commands

- Use the "Voice Input" button for speech recognition.
- Speak clearly into your microphone.
- Spoken words will be converted to text and processed.

## Controls

- **Send**: Sends your message to the OpenAI model.
- **Voice Input**: Initiates voice command recognition and sends your message to the OpenAI model.
- **Stop Speech**: Stops ongoing speech playback.
- **Clear**: Clears the chat history from the window but doesn't affect the context JSON.

## Troubleshooting

- Ensure your API key is valid and has necessary permissions.
- Verify your internet connection.
- For speech recognition, check microphone configuration.

## License

Licensed under the Apache 2.0 License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for the API.
- Google's gTTS and Speech Recognition for speech services.
- Pygame for audio handling.

---
