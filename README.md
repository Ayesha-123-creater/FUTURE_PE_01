# AI YouTube Script & Thumbnail Generator

A fully client-side web app that helps YouTubers generate **video scripts** and **thumbnails** using AI. Built with **HTML, TailwindCSS, and JavaScript**, it uses the **OpenAI API** for script generation and prompt creation.


## 🚀 Features

- 🎬 **AI Script Generator**
  - Generates YouTube video scripts with hooks, timestamps, CTAs, and B-roll suggestions.
  - Supports different tones (friendly, professional, humorous, motivational).
  - Adjustable length (short, medium, long).
  - One-click shorten or expand functionality.

- 🖼️ **Thumbnail Creator**
  - Draws a thumbnail preview on HTML5 Canvas.
  - Allows custom text and styles.
  - Generates a **detailed image prompt** for use in DALL·E, Midjourney, or Leonardo.ai.
  - Download or copy thumbnail PNG.

- 📋 **Utilities**
  - Copy or export generated scripts.
  - Copy prompts directly to clipboard.


## 🧠 Prompt Engineering Logic

The app uses carefully crafted prompts to guide the AI model. For example:

```text
You are a professional YouTube scriptwriter experienced at short and mid-form content.
Title: "Top 5 AI Tools for Students"
Keywords: AI tools, productivity, student hacks
Tone: Friendly & energetic
Target length: Medium

Produce:
- A short hook (2–4 lines) with on-screen hook suggestion.
- Sections with timestamps (Intro, Main points, Examples, Call to action).
- Shot suggestions (B-roll, on-screen text, cutaway).
- Suggested thumbnail text and 3 alternative video titles.
```

This prompt structure ensures **clarity**, **engagement**, and **reproducible output**, highlighting how prompt design affects AI responses.

---

## 🧩 Tech Stack
| Layer | Technology |
|--------|-------------|
| Frontend | HTML5, TailwindCSS |
| Logic | Vanilla JavaScript |
| AI Backend | OpenAI API (GPT-4o-mini) |
| Drawing | HTML Canvas |


## 🛠️ Setup Instructions

1. Clone or download this repository.
2. Open the `ai_youtube_generator.html` file in your browser.
3. Go to [https://platform.openai.com/api-keys](https://platform.openai.com/api-keys) and generate your **API key**.
4. Paste your API key into the app’s **OpenAI API Key** field.
5. Enter a video title, keywords, tone, and length.
6. Click **Generate Script** — your AI-generated YouTube script will appear!
7. Use the thumbnail tools to design and download thumbnails.


## 📄 Example Workflow

1. **Input:**
   - Title: `Top 5 AI Tools for Students`
   - Keywords: `AI, student productivity, tools`
   - Tone: `Friendly & energetic`

2. **Output:**
   - Hook: “Tired of spending hours on assignments? These 5 AI tools will save your semester!”
   - Timestamps: `0:00 Intro`, `0:45 Tool 1`, `1:20 Tool 2`, …
   - CTA: “Subscribe for more AI-powered study hacks!”

3. **Thumbnail Prompt:**
   - “Create a high-resolution YouTube thumbnail with large text '5 AI Tools for Students', bold lighting, friendly face on right side…”


## 🧑‍💻 How It Works

- The app sends a `fetch()` POST request to the OpenAI Chat Completion endpoint.
- The AI model responds with a structured YouTube script.
- Thumbnail and prompt generation are handled locally on the browser using Canvas and JavaScript.

## ⚙️ File Structure

/ (root)
│
├── index.html   # Main single-file app (HTML + CSS + JS)
└── README.md                   # Documentation (this file)


## 🔒 Security
- The API key is **never sent to any external server** — it is used directly in your browser.
- All generation happens client-side.

## 💡 Future Enhancements
- 🎙️ Voiceover + TTS export.
- 🧩 Auto YouTube description + hashtags.
- 🎨 Brand kit integration (fonts/colors).
- 🪄 AI thumbnail image generation via DALL·E API.



## 🏁 Author
Prompt Engineering & AI Application Development


## 📚 License
This project is open for educational use — feel free to customize and extend it for your AI coursework or YouTube automation projects.
