# Live Captioning with Real-Time Translation

## New Feature: Dynamic Multi-Language Translation

The live captioning application now includes real-time translation functionality that allows users to select both the source language for speech recognition and the target language for translation.

### Features Added

1. **Dynamic Language Selection**: Choose the language you're speaking in and the language you want to translate to
2. **Real-Time Translation**: As you speak, captions are automatically translated to your selected target language
3. **Visual Distinction**: The translation appears in a darker blue background to distinguish it from the original captions
4. **Live Language Switching**: Change languages on the fly without stopping the captioning session
5. **Debounced API Calls**: Translation requests are debounced to prevent excessive API calls
6. **Error Handling**: If translation fails, the original text is shown as fallback
7. **Responsive Design**: Works on both desktop and mobile devices

### How It Works

1. **Language Selection**: Choose your source language (what you're speaking) and target language (what you want to translate to)
2. **Speech Recognition**: The app captures your speech and converts it to text in your selected source language
3. **Translation**: The text is sent to Google Translate API for translation to your target language
4. **Display**: Both original and translated text are displayed simultaneously
5. **Real-Time Updates**: Both captions update in real-time as you speak
6. **Dynamic Switching**: Change languages on the fly - the app will restart recognition with the new source language

### Technical Details

- **Translation API**: Uses Google Translate's free API endpoint
- **Dynamic Language Support**: Supports 25+ languages for both speech recognition and translation
- **Live Language Switching**: Automatically restarts speech recognition when source language changes
- **Debouncing**: 500ms delay to prevent excessive API calls
- **Error Handling**: Graceful fallback to original text if translation fails
- **Responsive Design**: Adapts to different screen sizes
- **Styling**: Translation appears in a distinct dark blue background

### Usage

1. Open the application in Chrome browser
2. Select your **Speech Recognition Language** (the language you'll be speaking in)
3. Select your **Translation Language** (the language you want to translate to)
4. Click "Click to Caption" to start
5. Allow microphone access
6. Begin speaking - you'll see both original and translated captions
7. **Optional**: Change languages on the fly - the app will automatically restart with the new source language
8. Click the text to stop captioning

### Browser Requirements

- Chrome desktop browser (version 25+)
- Internet connection (required for translation API)
- JavaScript enabled
- Microphone access

### Notes

- Translation requires an internet connection
- The Google Translate API is free but has rate limits
- Translation quality depends on the clarity of speech and complexity of content
- Both English and Japanese transcripts are saved in the session data 