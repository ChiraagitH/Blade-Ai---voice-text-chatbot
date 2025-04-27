Blade Ai - LLaMA 3 Powered Chatbot with Voice Interaction
Blade Ai is a local chatbot powered by LLaMA 3, integrated with Gradio for a user-friendly interface and enhanced with voice input/output functionality. It runs locally on your system using Ollama for LLaMA 3 model hosting. This project aims to provide an interactive experience through text and voice, enabling seamless communication with LLaMA 3.

Features
Local LLaMA 3 Integration: The chatbot runs on LLaMA 3, a powerful language model, via Ollama on your local machine.

Voice Interaction: Use voice input and output to interact with the chatbot, enabling hands-free conversations.

Gradio UI: A simple and intuitive web interface built using Gradio for seamless interaction via text or voice.

Speech-to-Text & Text-to-Speech: Utilizes the speech_recognition library for converting speech to text and pyttsx3 for converting text to speech, offering offline capabilities.

Requirements
Before using Blade Ai, make sure you have the following installed:

Python 3.6 or higher

LLaMA 3 model running on Ollama locally

requests library

gradio library

speech_recognition library

pyttsx3 library

pyaudio library for microphone access

You can install the necessary libraries using pip:

bash
Copy
Edit
pip install requests gradio speechrecognition pyttsx3 pyaudio
Setup Instructions
Step 1: Install Dependencies
Make sure to install all the dependencies by running the following command:

bash
Copy
Edit
pip install -r requirements.txt
If requirements.txt is not available, manually install the necessary packages as mentioned above.

Step 2: Running the Local LLaMA 3 Server
You need to have LLaMA 3 running on your local server using Ollama. Ensure that the model is accessible on http://localhost:11434/api/generate.

Step 3: Start the Blade Ai Application
Once you have installed the required libraries and set up the LLaMA 3 server, you can start the Blade Ai application by running the following:

bash
Copy
Edit
python app.py
This will launch the Gradio interface on your local server. By default, the Gradio UI will be accessible at:

cpp
Copy
Edit
http://127.0.0.1:7860
You will be able to interact with the chatbot through either text or voice.

Step 4: Voice Interaction (Optional)
If you want to use voice interaction, make sure your microphone is connected and working. You can click on the 🎤 Voice Input button in the Gradio interface, and speak to interact with the chatbot.

Example Interaction
Text-based:

You type: "Hello, how are you?"

LLaMA 3 responds: "I am doing great! How about you?"

Voice-based:

You click on the 🎤 Voice Input button and speak: "What's the weather today?"

LLaMA 3 responds: "I'm sorry, I don't have access to real-time data, but you can check your local weather app."

Project Structure
bash
Copy
Edit
.
├── app.py              # Main application to run Gradio interface and voice integration
├── requirements.txt    # List of required Python packages
├── README.md           # This file
└── voice_interaction.py # Contains logic for speech-to-text and text-to-speech
Contributing
Feel free to fork this repository, make improvements, or fix any bugs you encounter. If you would like to contribute, please open a pull request with your proposed changes.

License
This project is open-source and available under the MIT License.

Customizing for Your Setup
If you're using a different local port or server setup for LLaMA 3, make sure to update the URL in the code where it sends requests to the local server:

python
Copy
Edit
response = requests.post(
    "http://localhost:11434/api/generate",  # Change port if necessary
    json={"model": "llama3", "prompt": prompt, "stream": False}
)
Troubleshooting
Gradio Interface Not Launching: Ensure that you have installed all dependencies and the LLaMA model is running locally.

Voice Input Issues: Make sure that your microphone is working correctly and accessible by Python. If you face issues with pyaudio, try reinstalling it or using an alternative microphone access library.

Acknowledgments
Ollama: For hosting LLaMA 3 locally.

Gradio: For creating an easy-to-use interface for web-based applications.

SpeechRecognition: For converting speech to text.

pyttsx3: For offline text-to-speech synthesis.

