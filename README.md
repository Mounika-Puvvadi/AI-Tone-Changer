---
title: tone_generator
app_file: openrouter_web_tonegenerator.py
sdk: gradio
sdk_version: 5.22.0
---
# OpenRouter Chatbot Implementations

This repository contains two implementations of chatbots using the OpenRouter API:

1. **Command-line Chatbot** (`openrouter_chatbot.py`)
2. **Web Interface Chatbot** (`openrouter_web_chatbot.py`)

Both implementations use the Deepseek AI model through OpenRouter and include rate limiting to prevent excessive API usage.

## Setup

1. **Install dependencies**:
   ```
   pip install -r requirements.txt
   ```

2. **Set up environment variables**:
   - Create a `.env` file in the project root with:
   ```
   OPENROUTER_API_KEY=your_api_key_here
   ```
   - Alternatively, set this environment variable through your system's settings

## Usage

### Command-line Chatbot

Run the command-line interface:
```
python openrouter_chatbot.py
```

Type your messages and press Enter. Type 'exit' to quit.

### Web Interface Chatbot

Run the web interface:
```
python openrouter_web_chatbot.py
```

This will start a local Gradio web server. Open the displayed URL in your browser to interact with the chatbot.

## Features

- **Rate Limiting**: Both implementations limit requests to 10 per minute by default
- **Response Cleanup**: Formats AI responses to be well-structured and complete
- **Chat History**: The web interface retains conversation history
- **Error Handling**: Graceful handling of API errors and timeouts

## Configuration

You can adjust the following settings in the code:
- `MAX_REQUESTS_PER_MINUTE`: Change the rate limit
- `MODEL`: Select a different model from OpenRouter
- `temperature` and other generation parameters in the API request

## License

MIT 