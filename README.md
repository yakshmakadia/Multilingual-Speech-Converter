#  Multilingual Text-to-Speech & Speech-to-Text Platform

A full-stack web app that enables:
✅ Text-to-Speech (TTS) in multiple languages  
✅ Speech-to-Text (STT) transcription  
✅ Seamless translation features

Built with:
- React + TypeScript frontend (shadcn/ui)
- Node.js + TypeScript backend with modular services
- Shared schemas for validation and consistency

---

##  Project Structure
client/
├── src/
│ ├── components/
│ │ ├── layout/ (Header, Footer)
│ │ └── ui/ (shadcn components, audio controls)
│ ├── hooks/ (speech recognition, TTS)
│ ├── lib/ (languages, utils, query client)
│ └── pages/ (home, text-to-speech, speech-to-text, translation)
server/
├── services/ (speech-service, translation-service)
├── index.ts (server entry point)
├── routes.ts (API routes)
└── storage.ts (file storage, caching)
shared/
└── schema.ts

yaml
Copy
Edit

---

##  Features
- 🌍 Multilingual TTS: Convert text into speech in your chosen language
- 🗣️ STT: Transcribe speech into text
- 🔄 Translate text between languages
- 🖌️ Beautiful UI with shadcn components
- ⚙ Modular, scalable architecture

---
##  Tech Stack
Frontend: React + TypeScript, shadcn/ui, TanStack Query
Backend: Node.js, Express, TypeScript
Speech: Google Cloud, Azure TTS/STT, Whisper etc.
Translation: googletrans / Google Translate API
Validation: Zod / Yup

Future Enhancements

Multiple voice options (male/female, accents)
Batch text/audio conversion
User accounts & history
Usage analytics
Mobile-first UI improvements

## 🚀 Getting Started

### 📦 Install dependencies
```bash
cd client
npm install

cd ../server
npm install
🏃 Run the app locally
Start backend
bash
Copy
Edit
cd server
npm run dev
Backend runs on: http://localhost:4000

Start frontend
bash
Copy
Edit
cd client
npm run dev
Frontend runs on: http://localhost:3000

🔧 Configuration
Add environment variables to:

client/.env.local

server/.env

Example:

env
Copy
Edit
# server/.env
GOOGLE_API_KEY=your_google_api_key
OPENAI_API_KEY=your_openai_api_key
