# 🥢 Saigon Restaurant Voice Chatbot

A local Vietnamese voice chatbot for Saigon-style restaurants. Supports voice-based interaction for booking tables, asking about menus, and general Q&A.

## ⚙️ Tech Stack

- 🧠 **LlamaIndex + Ollama**: Local LLM for dialogue understanding
- 🔎 **Qdrant**: Vector DB for memory / context storage (Docker)
- 🎤 **FasterWhisper**: Fast and accurate speech-to-text
- 🔊 **Google TTS**: Natural Vietnamese speech output
- 🎮 **Pygame**: Simple UI loop (no web API)

## 🚀 Run

1. Start Qdrant:

```bash
docker run -p 6333:6333 qdrant/qdrant

```

Start chatbot:
```bash
python app.py
```

🗂️ Structure
saigon-voicebot/
├── rag/
│   ├── AIVoiceAssistant.py
│   └── Menu.txt
├── app.py
├── voice_service.py
├── requirements.txt
├── README.md
├── .gitattributes
└── __pycache__/

📦 Requirements
```bash
pip install -r requirements.txt
