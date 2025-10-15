# 🤖 AI Chatbot — Text + Vision (TinyDolphin + EasyOCR)

This project is a **Streamlit-based AI assistant** that combines text-based chat and image text extraction (OCR).  
It uses the **TinyDolphin model** through Ollama for chat and **EasyOCR** for image understanding.  

---

## 🌟 Features
- 🧠 **AI Chat Interface** — Talk with the TinyDolphin model locally via Ollama.  
- 🖼️ **Image Text Extraction (OCR)** — Upload images and extract visible text using EasyOCR.  
- 💬 **Chat History** — Maintain your conversations with session state.  
- 🛑 **Stop Generation** — Interrupt model responses in real-time.  
- 🎨 **Custom UI Design** — Styled with CSS for a modern chat interface.  
- 🚀 **Streamed Responses** — Watch answers generate live.  

---

## 🧩 Tech Stack
| Component      | Description |
|----------------|-------------|
| Frontend/UI    | Streamlit |
| Backend Model  | Ollama running TinyDolphin |
| OCR Engine     | EasyOCR |
| Language       | Python 3.9+ |
| Libraries Used | streamlit, ollama, easyocr, Pillow, numpy, datetime |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/AI-Chatbot.git
cd AI-Chatbot
2. Install Dependencies
Make sure you have Python 3.9+ installed.

bash
Copy code
pip install -r requirements.txt
3. Install and Run Ollama
You need to have Ollama installed and the TinyDolphin model available locally.

Install Ollama → Ollama official site

Pull TinyDolphin Model

bash
Copy code
ollama pull tinydolphin
Run Ollama Server

bash
Copy code
ollama serve
This starts Ollama’s local API at http://localhost:11434.

▶️ Run the App
Once Ollama is running, start the Streamlit app:

bash
Copy code
streamlit run app.py
Then open the link shown in the terminal (usually http://localhost:8501).

🧠 How It Works
Chat Interface
Enter text in the chat input box.

The app sends your prompt to Ollama’s TinyDolphin model.

Responses are streamed and displayed live.

Image Upload (OCR)
Upload a .jpg or .png image.

EasyOCR extracts text and shows it in the chat.

Chat History
Conversations are stored using Streamlit’s session state.

You can start new chats or clear all history from the sidebar.

🧑‍💻 Author
Anshul Kaushal

💼 GitHub: Your GitHub Profile

📜 License
This project is licensed under the MIT License — feel free to use and modify it.
