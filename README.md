# Audio Translator


## Description
This repository contains the code for a near real-time voice translator built in Python and designed to run on Google Colab.
Workflow: record audio in the browser → convert to WAV → transcribe in Portuguese (Whisper) → translate to English, French, and German (multilingual model M2M100, via Hugging Face) → speech synthesis (gTTS) for each target language.

Goal: Demonstrate a practical solution integrating ASR (speech-to-text), NMT (neural machine translation), and TTS (text-to-speech), useful for international meetings, tourism, or language learning.
---

## Features
- Audio recording in the browser (MediaRecorder, JS)
- Conversion from .webm → .wav (mono/16kHz)
- Portuguese transcription (Whisper)
- Translation PT → EN/FR/DE (M2M100 multilingual model)
- Voice synthesis in EN/FR/DE (gTTS)
- Chunk-based processing (4–5s) for near real-time experience

## Technologies & Resources Used

- Python
- Google Colab
- ffmpeg (audio conversion)
- Whisper (ASR)
- Transformers + sentencepiece (Hugging Face, M2M100 translation)
- gTTS (TTS)
