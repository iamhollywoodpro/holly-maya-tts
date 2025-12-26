---
title: HOLLY MAYA1 Voice
emoji: 🎙️
colorFrom: purple
colorTo: pink
sdk: docker
app_port: 7860
pinned: false
---

# 🎙️ HOLLY TTS - Maya1 Voice Service

**Self-hosted Text-to-Speech microservice for HOLLY AI**

Powered by [Maya1](https://huggingface.co/maya-research/maya1) - the best open-source emotional voice AI.

---

## 🌟 Features

- **HOLLY's Signature Voice**: Female, 30s, American accent, confident, intelligent, warm tone
- **20+ Emotions**: `<laugh>`, `<chuckle>`, `<whisper>`, `<sigh>`, `<confident>`, etc.
- **24kHz Quality**: Professional broadcast-quality audio
- **Free & Open Source**: Apache 2.0 license, no API costs
- **Production-Ready**: FastAPI + Maya1 + SNAC codec
- **Streaming Ready**: Sub-100ms latency with vLLM (optional)

---

## 🚀 Quick Start

### **Local Development**

```bash
# Install dependencies
pip install -r requirements.txt

# Run the service
python app.py

# Test endpoint
curl -X POST http://localhost:7860/generate \
  -H "Content-Type: application/json" \
  -d '{"text": "Hello Hollywood! I am HOLLY."}' \
  --output test.wav
```

---

## 🎯 API Endpoints

### **POST /generate**
Generate speech from text (returns WAV audio)

### **GET /health**
Health check for monitoring

### **GET /voice/info**
Get HOLLY's voice profile

---

## 🎤 Emotion Tags

Add inline emotions to your text:

```
"Great work, Hollywood! <chuckle> That was impressive."
"Let me whisper this secret <whisper> between us."
```

**Supported emotions:**
- `<laugh>`, `<chuckle>`, `<whisper>`, `<sigh>`, `<confident>`, etc.

---

## 📝 License

**Apache 2.0** - Fully open source, commercial use allowed.

---

**🎙️ Give HOLLY her voice!**
