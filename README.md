# 📖 Dictionary App

A modern **Dictionary Web App** built with **HTML, TailwindCSS, and JavaScript**.  
This app allows users to **search for English words**, view **meanings, phonetics, synonyms, antonyms, audio pronunciation**, and even see **Bengali translations** (via Google Gemini API).  

---

## 🚀 Features

- 🔍 **Word Search** – Search for any English word using the [Free Dictionary API](https://dictionaryapi.dev/).  
- 📚 **Word Details** – Displays:
  - Phonetics (IPA notation)  
  - Audio pronunciation 🔊  
  - Definitions (multiple meanings)  
  - Synonyms & Antonyms  
  - Word forms (basic noun/verb forms)  
- 🌗 **Light/Dark Mode Toggle** – Remembers preference using **LocalStorage**.  
- 💡 **Smart Suggestions** – Autocomplete suggestions while typing.  
- 🌐 **Bengali Meaning** – Fetches a simple translation using **Google Gemini API** (requires your API key).  
- 🎨 **Responsive UI** – Clean and mobile-friendly design with **TailwindCSS**.  

---

## 📂 Project Structure

project/
│── index.html # Main application file
│── README.md # Documentation

yaml
 

---

## 🔧 Requirements

- A modern browser (Chrome, Edge, Firefox).  
- Internet connection (to fetch data from the Dictionary API and Gemini API).  
- (Optional) A **Google Gemini API key** for Bengali translation.  

---

## ▶️ Running the App

### Option 1: Open Directly
1. Download or clone this repository.  
2. Open `index.html` in your browser.  

### Option 2: Serve with Local Server (Recommended)
Use Python’s built-in HTTP server:  

```bash
# Python 3
python -m http.server 8080
Now visit:
👉 http://127.0.0.1:8080/index.html

⚙️ Setup Bengali Translation (Optional)
The app includes a function to fetch Bengali translations using Google Gemini API.

Get a free API key from Google AI Studio.

In the code, locate this section in index.html:

javascript
 
const apiKey = "";
Replace with your key:

javascript
 
const apiKey = "YOUR_GEMINI_API_KEY_HERE";
Now Bengali translations will appear under each word definition.

💻 Usage
Enter a word in the search bar (e.g., knowledge).

Hit Enter or click the Search button.

View:

Meaning

Pronunciation

Synonyms & Antonyms

Bengali Meaning (if enabled)

Toggle dark mode 🌙 / light mode ☀️ with the switch in the header.

Try typing ap and select from suggestions like apple.

📑 Example API Response (Dictionary API)
json
 
[
  {
    "word": "hello",
    "phonetic": "/həˈləʊ/",
    "phonetics": [{ "audio": "https://lex-audio..." }],
    "meanings": [
      {
        "partOfSpeech": "exclamation",
        "definitions": [{ "definition": "Used as a greeting." }],
        "synonyms": [],
        "antonyms": []
      }
    ]
  }
]
⚠️ Notes
The app relies on the free DictionaryAPI.dev.

Bengali translation requires a valid Gemini API key. If no key is provided, it will simply display "Translation not available."

Audio pronunciation may not be available for all words.

📜 License
This project is for educational purposes and is free to use.

