# Blade-Ai---voice-text-chatbot
import requests

while True:
    user_input = input("You: ")
    if user_input.lower() in ["exit", "quit"]:
        break

    try:
        response = requests.post(
            "http://localhost:11434/api/generate",
            json={
                "model": "llama3",
                "prompt": user_input,
                "stream": False
            },
            timeout=30
        )

        if response.status_code == 200:
            data = response.json()
            print("LLaMA 3:", data.get("response", "").strip())
        else:
            print("Error:", response.status_code, response.text)

    except requests.exceptions.RequestException as e:
        print("Request failed:", e)
