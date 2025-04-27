# Blade Ai - LLaMA 3 Powered Chatbot with Voice Interaction

Blade Ai is a local chatbot powered by the LLaMA 3 model, integrated with Gradio for a user-friendly interface and enhanced with voice interaction features. The chatbot runs on your local server using Ollama for LLaMA 3 hosting. Users can communicate with the chatbot through text or voice input and get responses via text or speech.

---

## 🚀 Features
- Local LLaMA 3 Integration: The chatbot runs the LLaMA 3 model locally via Ollama.
- Voice Interaction: Supports voice input and output for a more interactive experience.
- Gradio UI: Provides a simple web interface for both text and voice-based conversations.
- Speech-to-Text & Text-to-Speech: Offline conversion from speech to text using speech_recognition and text-to-speech using pyttsx3.

---

## Requirements
- Python 3.6+
- [SpeechRecognition](https://pypi.org/project/SpeechRecognition/)
- [pyttsx3](https://pypi.org/project/pyttsx3/)
- [Requests](https://pypi.org/project/requests/)
- gradio library
- Ollama (for local LLaMA model serving)



---

## ⚙️ How to Run

1. Install Ollama and pull LLaMA model locally:
    ```bash
    ollama pull llama3
    ollama run llama3
    ```

2. Install Python packages:
    ```bash
    pip install speechrecognition pyttsx3 requests
    ```

3. Clone this repo:
    ```bash
    git clone https://github.com/Chiraagith/Blade-Ai---voice-text-chatbot.git
    cd Blade-Ai---voice-text-chatbot
    ```

4. Run the script:
    ```bash
    python blade_ai_chatbot.py
    ```

5. Speak to your AI! 🎙️✨

---


