# Blade Ai - LLaMA 3 Powered Chatbot with Voice Interaction

**Blade Ai** is a local chatbot powered by the LLaMA 3 model, integrated with Gradio for a user-friendly interface and enhanced with voice interaction features. The chatbot runs on your local server using Ollama for LLaMA 3 hosting. Users can communicate with the chatbot through text or voice input and get responses via text or speech.

## Features

- **Local LLaMA 3 Integration**: The chatbot runs the LLaMA 3 model locally via Ollama.
- **Voice Interaction**: Supports voice input and output for a more interactive experience.
- **Gradio UI**: Provides a simple web interface for both text and voice-based conversations.
- **Speech-to-Text & Text-to-Speech**: Offline conversion from speech to text using `speech_recognition` and text-to-speech using `pyttsx3`.

## Requirements

- Python 3.6+
- LLaMA 3 model running on Ollama locally
- `requests` library
- `gradio` library
- `speech_recognition` library
- `pyttsx3` library
- `pyaudio` library for microphone access

### Installation

1. **Install Dependencies**:

   Use the following command to install the required Python packages:

   ```bash
   pip install requests gradio speechrecognition pyttsx3 pyaudio

2. **Set Up LLaMA 3 Locally**:

   Make sure to have LLaMA 3 running on your local machine via Ollama. The model should be 
   accessible at:

   ```bash
   http://localhost:11434/api/generate

## Setup Instructions

### Step 1: Install Dependencies

Install all the necessary dependencies by running:

### Step 2: Run the Blade Ai Application

Once all the dependencies are installed, run the Blade Ai application

### Step 3: Voice Interaction (Optional)

Ensure your microphone is set up and working. You can use voice input by clicking the 🎤 Voice Input button in the Gradio interface. The chatbot will listen to your voice input, convert it to text, and respond via text-to-speech.
 
  ```bash
  pip install -r requirements.txt
  pip install requests gradio speechrecognition pyttsx3 pyaudio

  step 2:
  python app.py
  
  
  
   
