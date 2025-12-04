⚔️ Kimetsu no Yaiba Companion App

"Set your heart ablaze!" ❤️‍🔥

A fan-made, immersive interactive companion app built with React + Vite + Tailwind. Explore character lore, play mini-games, and chat with Hashira, Demons, and the Main Squad in an in-character messenger-style experience.

🔗 Live Demo

[👉 Click here to enter the Infinity Castle](https://kimetsu-no-yoiba.netlify.app/)

✨ Key Features

🧭 Main Sections

Home: Atmospheric landing page with anime-style backgrounds and cinematic intro vibes.

Encyclopedia: Detailed character cards with images, roles, and lore. Includes direct entry to the "Chat" system from any character profile.

Games / Activities: Interactive mini-games themed around Demon Slayer training and breathing styles.

Messages (Messenger Crow): A dedicated inbox-style page featuring a 2-column layout.

Left: Scrollable character list.

Right: Chat guidance/placeholder.

Theme: Set against a mystical library/messenger background.

🗣️ Advanced Character Chat System

Immersive UI: A nearly full-screen CharacterChatModal designed to feel like a modern game companion interface.

Context Awareness: The AI remembers conversation history for a natural flow.

In-Character Personalities: Each major character has a dedicated system prompt via getCharacterPrompt(char) ensuring they act authentically:

Zenitsu: Randomly screams about Nezuko and marriage.

Inosuke: Mangles names ("Gonpachiro!") and shouts about being the God of Mountains.

Rengoku: Ends sentences with "!!" and talks about setting your heart ablaze.

Uzui: Obsessed with everything being FLASHY.

Muzan/Akaza/Doma: Villain-appropriate, chilling or arrogant responses.

🧠 Persistent Chat History

Seamless Experience: The app uses a centralized chatHistories state.

Cross-Feature Sync: Chat history is shared between the Encyclopedia "Chat" button, the Profile page, and the Messages inbox. When you reopen a chat, your previous conversation is right there.

🛡️ Robust Fallback System (Offline Mode)

Even if the AI API hits a limit or network error, the immersion never breaks.

Per-Character Fallbacks: 20–30+ hand-crafted lines for every single character that match their personality perfectly.

Roleplay Ready: Even without the live model, the app feels like a character.ai style roleplay experience using these dynamic quotes.

🎥 Cinematic Experience

Dynamic Intro: "BGMI-style" 10-second video intro with a "Tap to Start" mechanic to bypass browser autoplay restrictions.

Immersive Audio: Background theme music (theme.mp3) loops automatically, with a global floating mute toggle.

Visuals: Dynamic background switching based on the active screen (Infinity Castle, Wisteria Mansion, etc.) using optimized .webp assets for fast loading.

🛠️ Tech Stack

Frontend: React.js (v18)

Build Tool: Vite

Styling: Tailwind CSS (Custom animations, filters, glassmorphism)

AI Integration: Google Gemini API (with robust fallbacks)

State Management: React Hooks (useState, useEffect, useRef)

Assets: WebP optimized images and video integration

🚀 Running Locally

To run this project on your local machine, follow these steps:

Clone the repository

git clone [https://github.com/SanikaTribhuvan/demon-slayer-app.git](https://github.com/SanikaTribhuvan/demon-slayer-app.git)
cd demon-slayer-app


Install Dependencies

npm install


Set up Environment Variables
Create a .env file in the root directory and add your API key:

VITE_GEMINI_API_KEY=your_api_key_here


Run the Development Server

npm run dev


Open in Browser
Visit http://localhost:5173 to view the app.

📂 Project Structure

demon-slayer-app/
├── public/
│   ├── audio/           # Theme music files
│   ├── backgrounds/     # High-res WebP wallpapers
│   ├── images/          # Character portraits (WebP)
│   ├── videos/          # Intro video clips
│   └── logo.png         # Official Logo
├── src/
│   ├── App.jsx          # Main Application Logic & Chat System
│   ├── index.css        # Tailwind imports & Custom Fonts (Cinzel)
│   └── main.jsx         # Entry point
└── tailwind.config.js   # Tailwind configuration
