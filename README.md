# Blade-Ai---voice-text-chatbot

A LLaMA3-powered chatbot that uses **voice recognition** and **text-to-speech** to have full conversations with an AI model running locally via **Ollama**.

---

## 🚀 Features
- 🎤 Voice Input using Microphone
- 🧠 Smart Responses powered by LLaMA 3 (via Ollama)
- 🔊 Voice Output (AI talks back to you)
- 🛑 Say "exit" to end the conversation
- 🖥️ Runs locally, no internet needed for model inference

---

## 📦 Technologies Used
- Python
- [SpeechRecognition](https://pypi.org/project/SpeechRecognition/)
- [pyttsx3](https://pypi.org/project/pyttsx3/)
- [Requests](https://pypi.org/project/requests/)
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

## 📄 Project Structure

