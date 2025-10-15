# 🤖 AI Chatbot with OCR

This project is a custom-built **AI Chatbot using Streamlit**. It integrates a powerful local language model, **Tiny Dolphin**, served via **Ollama**, and includes **Optical Character Recognition (OCR)** capabilities provided by **EasyOCR**.

This application allows users to:
- Engage in interactive conversations with the Tiny Dolphin AI model.
- Upload images (`.png`, `.jpg`) to automatically extract text.
- Use the extracted text as context for questions.
- Manage and revisit past conversations through a session-based chat history.
- Enjoy a clean, custom-styled interface for a polished user experience.

---

## 🌟 Features

- 🧠 **Interactive AI Chat** — Have dynamic conversations with the Tiny Dolphin model running locally.
- 🖼️ **Image Text Extraction (OCR)** — Upload an image, and the app uses EasyOCR to read and extract any text within it.
- 💬 **Context-Aware Conversations** — Ask questions directly related to the text extracted from your uploaded images.
- 📜 **Chat History** — The sidebar keeps a log of your recent conversations, which you can revisit or clear.
- ✨ **Custom UI/UX** — A unique theme and modern chat components styled with custom CSS for a great look and feel.
- 🚀 **Built with Python** — A pure Python implementation leveraging powerful libraries for AI and web development.

---

## 🧩 Tech Stack

| Component | Description |
|---|---|
| **Frontend/UI** | [Streamlit](https://streamlit.io) |
| **Backend AI Model** | [Ollama](https://ollama.ai) running **Tiny Dolphin** |
| **OCR Engine** | [EasyOCR](https://github.com/JaidedAI/EasyOCR) |
| **Language** | Python 3.9+ |
| **Core Libraries** | `streamlit`, `ollama`, `easyocr`, `Pillow`, `numpy` |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone [https://github.com/Anshulkaushal01/AI_Chatbot.git]
cd ai_chat.py
```

### 2. Install Dependencies
Make sure you have Python 3.9+ installed.

```bash
pip install streamlit requests
```

### 3. Install the main Python libraries

```bash
pip install streamlit ollama easyocr
```

### 4. EasyOCR may require you to install PyTorch separately.
Visit [https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/) for instructions.

### 4. Install and Run Ollama
You need to have Ollama installed and the **Tiny Dolphin model** available locally.

### 5. Install Ollama
Visit Ollama’s official website to download and install it.

### 6. Pull the Tiny Dolphin Model
```Bash
ollama pull tinydolphin
```
#### Run the Ollama Server
Keep this running in a separate terminal.

```Bash
ollama serve
```
This starts Ollama’s local API, which the app will connect to.

---

### ▶️ Run the App

Once Ollama is running, start the Streamlit application:

```Bash
streamlit ai_chat.py
```

Now, open the local URL shown in your terminal (usually http://localhost:8501) in your web browser.

## 🧠 How It Works
  
  1. **Chat Interface**
     - Users type messages into the chat input.
     - The app sends the prompt to the local Tiny Dolphin model via the Ollama API.
     - The model's response is displayed in the chat window.

  2. **Image Upload & OCR**
     - A user uploads a .jpg or .png image.
     - EasyOCR processes the image locally to extract all visible text.
     - The extracted text is displayed in a message and is automatically pre-pended as context to the user's next chat message.
       
  3. **Chat History**
     - Conversations are stored in Streamlit’s session state.
     - You can start a new chat, which archives the current one, or view previous chats by clicking on them in the sidebar.

## 🧑‍💻 Author

**Anshul Kaushal**

---

## 📜 License
This project is licensed under the MIT License. Feel free to use, modify, and distribute it as you see fit.

---
