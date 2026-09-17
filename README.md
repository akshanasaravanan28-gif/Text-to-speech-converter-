# Text-to-Speech Converter 🔊📝

A single-screen Android app, built with **MIT App Inventor**, that converts any text a user types into spoken audio using the device's built-in text-to-speech engine.

## How it works

1. The user types any text into the **TextBox**
2. Tapping the **Speak** button reads the text box contents aloud
3. The `TextToSpeech1` component converts the entered text into speech
4. The device's built-in text-to-speech engine produces the spoken output
5. The user can edit or clear the text and enter a new message
6. Tapping **Speak** again reads the updated text aloud

## Features

- 📝 Simple text input field for typing any message
- 🔊 One-tap conversion of typed text into spoken audio
- 🗣️ Uses the device's built-in Text-to-Speech engine
- ⚡ Converts text to speech instantly
- 🖥️ Minimal, single-screen interface
- 📱 Built completely using MIT App Inventor's block-based programming

## Tech Stack

- **Platform:** MIT App Inventor (block-based, no native code)
- **Components:** `Button1` (Speak button), `TextBox1` (text input), `TextToSpeech1` (non-visible TTS component)
- **Blocks logic:** A single event handler is used to pass the text from `TextBox1` to `TextToSpeech1`
- **Programming:** MIT App Inventor Blocks

## How the Blocks Work

| Event / Component | Action |
|---|---|
| `Button1.Click` | Gets the text from `TextBox1` and passes it to `TextToSpeech1.Speak` |
| `TextBox1.Text` | Provides the text entered by the user |
| `TextToSpeech1.Speak` | Converts the text into spoken audio using the device's TTS engine |

## Example

| Action | Result |
|---|---|
| Type `"Hello world"` in the text box | Text box contains `"Hello world"` |
| Tap **Speak** | Device speaks `"Hello world"` aloud |
| Clear the text box and type new text | New text is ready to be spoken |
| Tap **Speak** again | Device speaks the new text aloud |

## Screenshot

![App Screenshot]IMG-20260917-WA0004.jpg)

*The app interface showing the text input field and Speak button.*

## Limitations (v1.0)

- No language or locale picker
- Uses the available device TTS voice
- No pitch control
- No speech-rate control
- No history of previously spoken text
- No error handling for empty text input

## Future Improvements

- Add a language/locale picker for different languages
- Add pitch and speech-rate controls
- Add a **Clear** button to reset the text box
- Save recently spoken phrases using TinyDB
- Add a warning when the text box is empty
- Add multiple voice options
- Improve the user interface and overall user experience

---
*Built as a mini project — MIT App Inventor, block-based development.*
