# Jarvis Voice Assistant

A Python-based voice assistant that can perform various tasks through voice commands, including web browsing, music playback, news updates, and AI-powered conversations using Google's Gemini API.

## Features

- **Voice Activation**: Activated by saying "Jarvis"
- **Web Navigation**: Open popular websites like Google, Facebook, YouTube, and LinkedIn
- **Music Playback**: Play songs from a predefined YouTube music library
- **News Updates**: Get the latest news headlines using NewsAPI
- **Web Search**: Perform Google searches through voice commands
- **Weather Information**: Get current weather updates for specified cities
- **AI Conversations**: Engage in natural conversations using Google's Gemini AI

## Prerequisites

```bash
pip install speech_recognition
pip install pyttsx3
pip install requests
pip install google-generativeai
```

## API Keys Required

- NewsAPI Key: Required for fetching news headlines
- Google Gemini API Key: Required for AI conversations
- OpenWeatherMap API Key: Required for weather information

## Installation

1. Clone the repository:
```bash
git clone [your-repository-url]
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

3. Configure API keys in the script:
```python
newsapi_key = "your_newsapi_key"
gemini_api_key = "your_gemini_api_key"
# Add weather API key in the weather section
```

## Usage

1. Run the script:
```bash
python jarvis.py
```

2. Wake up Jarvis by saying "Jarvis"
3. After activation, speak your command

## Available Commands

- **Open Websites**:
  - "Open Google"
  - "Open Facebook"
  - "Open YouTube"
  - "Open LinkedIn"

- **Music Playback**:
  - "Play [song_name]" (Available songs: jersey, abhi, harima, wolf)

- **Web Search**:
  - "Search [query]"

- **News**:
  - "News" (Gets top 5 headlines)

- **Weather**:
  - "Weather in [city_name]"

- **General Conversation**:
  - Any general query will be processed by the Gemini AI

## Music Library

Currently includes the following songs:
- Jersey
- Abhi
- Harima
- Wolf

## Error Handling

The assistant includes error handling for:
- Speech recognition timeout
- Unrecognized audio
- API request failures
- General exceptions

## Technical Details

- Uses `speech_recognition` for voice input
- `pyttsx3` for text-to-speech output
- Google's Speech Recognition API for command interpretation
- Gemini API for natural language processing
- NewsAPI for news updates
- OpenWeatherMap API for weather information

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details

## Acknowledgments

- Google Gemini API for AI capabilities
- NewsAPI for news services
- OpenWeatherMap for weather data

## Future Improvements

- Add more music library entries
- Implement custom wake word options
- Add support for more web services
- Implement local file operations
- Add calendar integration
- Expand AI capabilities

## Troubleshooting

If you encounter issues:
1. Check if all required packages are installed
2. Verify API keys are valid
3. Ensure microphone permissions are granted
4. Check internet connection
5. Verify Python version compatibility (Python 3.6+)
