## ✨ Ever overthink a simple message?
### You know... rereading it five times, wondering:
> “Does this sound too cold?”

> “Too formal?”

> “Too *me*?”
 
Welcome to the social anxiety zone. 😬

Whether you're texting a crush, replying to your boss, or just rewording that "Hey, just checking in" for the seventh time —
🎉 Meet your new messaging buddy: **the AI Tone Generator**.

It tweaks your words, smooths your vibe, and makes sure your tone hits just right — every time.

## **Stop second-guessing. Start sounding *exactly* how you want!** 💬💫

![image](https://github.com/user-attachments/assets/86758563-55d7-4491-9201-f5524e6461e8)

## Try It Out!

### [Try this AI tone generator RIGHT HERE! 🎭](https://huggingface.co/spaces/natgluons/tone_generator)

## Snapshots of the app in action
### Be friendly! :)
![image](https://github.com/user-attachments/assets/98135d41-1eb4-4170-a382-ddd0d0d9e998)
### Be casual~
![image](https://github.com/user-attachments/assets/d4d6988a-0978-468c-aa7b-fae0e7ac87aa)
### Be... playful?
![image](https://github.com/user-attachments/assets/33f7ba30-26ce-43bb-9155-80948e96635e)
### Or choose to be whatever you want!
![image](https://github.com/user-attachments/assets/0ad1271d-67a6-4ce0-ac38-e2d939d52816)
### Example prompt provided
![image](https://github.com/user-attachments/assets/fad26112-9f76-44bb-a6f6-a0f7dfcdf6b8)

### Have fun! ✨


---


# OpenRouter Chatbot Implementations
#### title: tone_generator | app_file: openrouter_web_tonegenerator.py | sdk: gradio | sdk_version: 5.22.0

This repository contains three implementations of chatbots using the OpenRouter API:

1. **Command-line Chatbot** (`openrouter_chatbot.py`)
2. **Web Interface Chatbot** (`openrouter_web_chatbot.py`)
3. **Web Interface AI Tone Generator** (`openrouter_web_tonegenerator.py`)

All implementations use the Deepseek V3 model through OpenRouter and include **rate limiting** to keep things fun and **fair**! (though let's normalize not hogging random people's API, please! We're all broke).

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

### Web Interface AI Tone Generator

Run the web interface:
```
python openrouter_web_tonegenerator.py
```


This will start a local Gradio web server. Open the displayed URL in your browser to interact with the chatbot.

## Features

- **Rate Limiting**: Both implementations limit requests to 10 per minute and 100 per day by default
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
