# 🩺 SympForYou — AI-Powered Multi-Channel Health Assistant

> **Live Demo:** [sympforyou.vercel.app](https://sympforyou.vercel.app/)

An intelligent, voice-enabled health assistant that orchestrates **IBM Watsonx (Granite)**, **NLU**, and **Speech services** to deliver real-time symptom analysis, drug information, and medical insights — across **Web** and **WhatsApp** platforms, in **12+ languages**.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🤒 **Symptom Analysis** | Describe symptoms in natural language and get AI-driven health insights |
| 💬 **AI Doctor Chat** | Conversational interface powered by IBM Granite LLM |
| 💊 **Drug Information** | Search any medication for its uses, indications, and guidance |
| 🗣️ **Voice I/O** | Speak your symptoms; get responses read aloud via IBM Speech services |
| 📱 **WhatsApp Integration** | Access the assistant directly on WhatsApp — no app install needed |
| 🌍 **Multilingual** | 12+ languages including Hindi, Arabic, Japanese, Chinese & more |
| 🔗 **WHO Resources** | Direct links to authoritative WHO health topics |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | TypeScript, Vercel |
| Backend | Python, Flask |
| LLM | IBM Watsonx.ai (Granite) |
| NLU | IBM Watson Natural Language Understanding |
| Voice Input | IBM Speech-to-Text API |
| Voice Output | IBM Text-to-Speech API |
| Messaging | WhatsApp Business API |

---

## 🌐 Supported Languages

🇺🇸 English · 🇪🇸 Spanish · 🇫🇷 French · 🇩🇪 German · 🇮🇳 Hindi · 🇧🇷 Portuguese  
🇮🇹 Italian · 🇯🇵 Japanese · 🇰🇷 Korean · 🇨🇳 Chinese · 🇳🇱 Dutch · 🇸🇦 Arabic

---

## 🏗️ Architecture
```
User (Web / WhatsApp)
        │
        ▼
  TypeScript Frontend (Vercel)
        │
        ▼
   Flask Backend (Python)
        │
   ┌────┴──────────────────────┐
   │                           │
IBM Watsonx.ai (Granite)   IBM NLU
IBM Speech-to-Text         IBM Text-to-Speech
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Node.js 18+ (for TypeScript)
- IBM Cloud account with:
  - Watsonx.ai
  - Watson NLU
  - Speech-to-Text
  - Text-to-Speech
- WhatsApp Business API credentials *(for WhatsApp channel)*

### 1. Clone the Repository
```bash
git clone https://github.com/VedantPandhare/IBM_sympchecker.git
cd IBM_sympchecker
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
npm install
```

### 3. Configure Environment Variables

Create a `.env` file:
```env
# IBM Watsonx.ai
WATSONX_API_KEY=your_watsonx_api_key
WATSONX_PROJECT_ID=your_project_id
WATSONX_URL=https://us-south.ml.cloud.ibm.com

# IBM NLU
NLU_API_KEY=your_nlu_api_key
NLU_URL=your_nlu_service_url

# IBM Speech-to-Text
STT_API_KEY=your_stt_api_key
STT_URL=your_stt_service_url

# IBM Text-to-Speech
TTS_API_KEY=your_tts_api_key
TTS_URL=your_tts_service_url

# WhatsApp
WHATSAPP_TOKEN=your_whatsapp_token
WHATSAPP_PHONE_ID=your_phone_number_id
```

### 4. Run
```bash
python app.py
```

---

## 🔑 IBM API Setup

1. Log in to [IBM Cloud](https://cloud.ibm.com)
2. Provision **Watsonx.ai**, **NLU**, **Speech-to-Text**, and **Text-to-Speech**
3. For each: **Manage → Credentials** → copy **API Key** and **Service URL**
4. For Watsonx.ai, copy your **Project ID** from the [dashboard](https://dataplatform.cloud.ibm.com)

---

## ⚠️ Disclaimer

> SympForYou is for **informational purposes only** and does not constitute professional medical advice. Always consult a qualified healthcare professional.

---

## 🙌 Acknowledgements

- [IBM Watsonx.ai (Granite)](https://www.ibm.com/watsonx)
- [IBM Watson NLU](https://www.ibm.com/cloud/watson-natural-language-understanding)
- [IBM Speech Services](https://www.ibm.com/cloud/watson-speech-to-text)
- [World Health Organization](https://www.who.int/health-topics)
