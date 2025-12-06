# Amharic-Video-Translator

🎧 Amharic Real-Time Dubbing Chrome Extension

AI-powered real-time translation for streaming platforms

This Chrome extension enables users to watch English-language movies and shows on platforms like Netflix, Amazon Prime Video, Hulu, and others with Amharic audio dubbing generated in real time.

The extension captures the audio from the streaming tab, sends it through an AI pipeline for speech recognition → translation → text-to-speech, and plays back synchronized Amharic audio to the user.

🚀 Features

Real-time audio capture using Chrome’s tabCapture API

AI speech recognition to convert English dialogue to text

Machine translation from English → Amharic

AI text-to-speech to generate natural Amharic audio

Synchronized playback over or instead of original audio

Simple pop-up UI to toggle translation on/off and change language settings

🧠 How It Works (Pipeline)

Capture Tab Audio
The extension listens to audio from the currently active video tab.

Speech-to-Text (STT)
Captured audio is streamed to a cloud provider (e.g., Google Cloud Speech-to-Text, Azure Speech Services).

Translate to Amharic
The recognized English text is translated to Amharic using a translation API.

Text-to-Speech (TTS)
The translated text is synthesized into spoken Amharic audio.

Playback
The extension uses Web Audio API to play the Amharic audio in sync with the video.

🧩 Tech Stack

Chrome Extensions (Manifest V3)

Chrome Tab Capture API

Web Audio API

Google Cloud / Azure for STT, Translation, and TTS

Node.js backend (optional) for streaming/chunk processing

JavaScript / TypeScript for extension logic

📦 Core Components
/extension
  ├── manifest.json
  ├── background.js (tab capture + audio routing)
  ├── popup.html / popup.js (UI)
  ├── translator.js (API integration)
  └── audioEngine.js (playback & sync)

 Add language selector

 Add optional subtitles in Amharic

 Release MVP
