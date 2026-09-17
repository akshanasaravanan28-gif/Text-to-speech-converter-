Text to Speech Converter

A simple Android app built with MIT App Inventor that converts typed text into spoken audio.

Overview

This app lets a user type any text into a text box and tap a button to have it read aloud using the device's built-in text-to-speech engine.

Features
Simple, single-screen interface
Type any text and convert it to speech instantly
Uses the device's native TTS engine (works offline once language data is installed)
Components Used
Component	Type	Purpose
Button1	Button	Triggers the text-to-speech conversion
TextBox1	TextBox	Input field where the user types text
TextToSpeech1	TextToSpeech	Converts the input text into spoken audio
How It Works (Blocks Logic)
when Button1.Click
do
   call TextToSpeech1.Speak
        message = TextBox1.Text

When the user taps Button1, the app calls TextToSpeech1.Speak, passing in whatever text is currently in TextBox1 as the message. The device then reads that text aloud.

Setup / How to Use
Open the project in MIT App Inventor.
Go to the Designer view and confirm the following components are on Screen1:
A Button
A TextBox
A TextToSpeech (non-visible component)
Switch to the Blocks view and set up the logic shown above.
Connect a device or emulator via Connect (AI Companion, USB, or Emulator).
Type text into the text box and tap the button to hear it spoken.
Possible Enhancements
Add a language/locale picker for TextToSpeech1
Add a pitch/speech-rate slider
Add a "Clear" button to reset the text box
Save recently spoken text to a list using TinyDB
Add error handling for empty text input
Requirements
MIT App Inventor account (web-based, no local install needed)
Android device or emulator with TTS support for testing
License

Free to use and modify for personal or educational purposes.

Content
