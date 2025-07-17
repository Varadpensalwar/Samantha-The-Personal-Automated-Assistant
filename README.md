# Samantha: The Personal Automated Assistant

## Live Demo

[[Samantha Bot](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT).


## Overview

Samantha is a sophisticated, AI-powered personal assistant inspired by the movie "Her". This project implements a versatile automated assistant that interacts through Telegram, processes both text and voice messages, and responds with natural, personalized communication using state-of-the-art language models.

## Features

- **Voice Recognition**: Processes voice messages sent via Telegram with high accuracy
- **Text-to-Speech**: Converts AI responses to natural-sounding voice using ElevenLabs API
- **Natural Conversation**: Engages in contextually aware, personalized dialogue
- **Email Integration**: Reads and composes emails through Gmail API integration
- **Calendar Management**: Accesses and manages Google Calendar events seamlessly
- **Calculation Tools**: Performs complex calculations and data processing on demand

## Technical Architecture

- **Telegram Bot API**: Secure interface for user interaction
- **OpenAI API**: Powers voice transcription and advanced text generation
- **DeepSeek AI**: Alternative language model for enhanced conversation capabilities
- **ElevenLabs API**: High-quality text-to-speech conversion
- **n8n Workflow Engine**: Orchestrates the entire process flow with reliability and scalability

## Installation & Setup

### Prerequisites

- [n8n](https://n8n.io/) workflow automation platform (v0.214.0 or higher)
- API keys for all integrated services
- Node.js (v16 or higher)

### Setup Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/Varadpensalwar/Samantha-The-Personal-Automated-Assistant.git
   ```

2. Import the `Samantha_Voice_Agent.json` file into your n8n instance

3. Configure the required API credentials:
   - Telegram Bot API
   - OpenAI API
   - DeepSeek API
   - ElevenLabs API
   - Gmail OAuth2 (for email functionality)
   - Google Calendar OAuth2 (for calendar management)

## Usage

Once deployed, you can interact with Samantha through your Telegram bot:

### Text Interaction
```
You: What's on my calendar today?
Samantha: [Provides calendar information with a personalized touch]
```

### Voice Interaction
- Send a voice message to your Telegram bot
- Samantha will transcribe your message, process it, and respond with both text and voice

### Supported Commands
- Calendar queries: "What's on my schedule tomorrow?"
- Email management: "Check my unread emails" or "Send an email to [recipient]"
- General questions: "What's the weather like?" or "Calculate 15% of 230"

## Customization

The assistant's personality and behavior can be extensively customized by modifying the prompt templates in the workflow:

### Personality Configuration
Edit the system prompts in the `Sam's Note` node to adjust:
- Response style and tone
- Conversation patterns
- Personality traits

### Current Personality Settings
The default configuration creates an assistant that provides:
- Warm, witty responses with natural conversational flow
- Personalized interactions (addressing the user by name)
- Concise communication (two sentences maximum)
- A balance of helpfulness and emotional intelligence

### Advanced Customization
For deeper customization, you can modify:
- The AI models used (in the OpenAI and DeepSeek nodes)
- Voice characteristics (in the ElevenLabs configuration)
- Workflow logic for specialized use cases

## License

This project is open source under the [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Acknowledgments

- Inspired by the AI character "Samantha" from the movie [Her](https://www.imdb.com/title/tt1798709/)
- Built using [n8n](https://n8n.io/) workflow automation
- Powered by [OpenAI](https://openai.com/), [DeepSeek](https://www.deepseek.com/), and [ElevenLabs](https://elevenlabs.io/) APIs

## Contact

Varad Pensalwar - [@varadpensalwar](https://github.com/Varadpensalwar)
