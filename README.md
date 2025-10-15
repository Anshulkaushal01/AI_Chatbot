🤖 AI Chatbot — Chat + OCR Assistant

This project is a Streamlit-based AI assistant that combines text-based chat with image text extraction (OCR) using the tinydolphin model via Ollama and EasyOCR.

It allows users to:

💬 Chat with an AI model locally via Ollama (tinydolphin).

🖼️ Upload an image and automatically extract text using EasyOCR.

📜 Maintain chat history with session state.

🎨 Interact via a clean, modern chat interface styled like ChatGPT.

🌟 Features

🧠 AI Chat Interface — Interact with the tinydolphin model directly from the browser.

🖼️ Image Text Extraction (OCR) — Upload images and extract text instantly using EasyOCR.

💬 Chat History — Save, view, and restore previous conversations.

🗑️ Clear History — Reset or start a fresh chat anytime.

🎨 Custom UI Design — Enhanced with CSS for a ChatGPT-like look.

🚀 Responsive Layout — Works smoothly on both desktop and mobile.

🧩 Tech Stack
Component	Description
Frontend/UI	Streamlit
Backend Model	Ollama running tinydolphin
OCR Engine	EasyOCR
Language	Python 3.9+
Libraries Used	streamlit, ollama, easyocr, Pillow, numpy, datetime
⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/yourusername/AI-Chatbot.git
cd AI-Chatbot

2️⃣ Install Dependencies

Make sure you have Python 3.9+ installed.
Install required libraries:

pip install -r requirements.txt


requirements.txt example:

streamlit==1.50.0
ollama
easyocr==1.7.2
Pillow==10.0.0
numpy==1.24.0

3️⃣ Install and Run Ollama

Download and install Ollama from its official website
.

Pull the tinydolphin model:

ollama pull tinydolphin


Start Ollama server:

ollama serve


This starts the local API at http://localhost:11434.

4️⃣ Run the App

Start the Streamlit chatbot:

streamlit run app.py


Then open the link shown in the terminal (usually http://localhost:8501
).

🧠 How It Works
🔹 Chat Interface

Type your message in the chat box.

The app sends your input to the tinydolphin model via Ollama API.

Responses are displayed in a chat-style UI.

🔹 Image Upload (OCR)

Upload a .jpg, .jpeg, or .png file.

The app uses EasyOCR to extract text.

Extracted text appears as a user message in the chat.

🔹 Chat History

Conversations are stored using Streamlit session state.

You can start new chats or clear all history from the sidebar.

🧑‍💻 Author

Anshul Kaushal

💼 GitHub: yourusername

📜 License

This project is licensed under the MIT License — feel free to use and modify it.
