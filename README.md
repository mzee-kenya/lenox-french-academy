Kirinyaga French Academy — Presentation Guide

Overview
- This is a small static mini-site demonstrating beginner French lessons (A1-A2).
- Open `index.html` in your browser to begin the demo.

Presentation Flow
1. Start at `index.html` to introduce the course levels and learning goals.
2. Click "Start Learning" to open `topics/a1-01-alphabet.html` and demo the interactive alphabet.
3. Use the "View All Topics" (`topics.html`) to show the structure and locked progression idea.
4. Navigate through `topics/` pages to demonstrate greetings, introductions, numbers, verbs, and daily activities.

Notes for demonstrator
- The pages use the Web Speech API (SpeechSynthesis) to play French pronunciations. Use a modern browser (Chrome, Edge, or Firefox) with voice support for `fr-FR`.
- Some example unlock logic uses `localStorage` keys (e.g. `a1-02-unlocked`) to illustrate progression. You can set these keys in the browser console during the demo, e.g.: `localStorage.setItem('a1-02-unlocked','true')`.

Files of interest
- `index.html` — Landing page with quick navigation.
- `topics.html` — Index of all topics (A1-B2 grouping).
- `topics/a1-01-alphabet.html` — Interactive alphabet and quiz.
- `topics/a1-02-greetings.html` — Greetings with conversation practice and audio.
- `topics/a1-03-introductions.html` — Introductions and self-introduction examples.
- `topics/a1-04-numbers.html` — Numbers with audio repetition practice.
- `topics/a1-05-basic-verbs.html` — Basic verbs and conjugation examples.
- `topics/a2-01-daily-activities.html` — A2 vocabulary table and quiz.

How to run locally
- Method 1 (quick): Double-click `index.html` to open in your default browser.
- Method 2 (recommended for SpeechSynthesis voices): Serve files with a simple static server to avoid any browser file-protocol limitations. Example using Python 3:

```bash
python -m http.server 8000
# then open http://localhost:8000/index.html
```

Presentation tips
- Mention that this is a minimal prototype focusing on content and pedagogy rather than full production features.
- Use the quiz and localStorage-based unlock to demonstrate a basic learner progression model.
- Explain speech playback may depend on installed OS/browser voices for French.

License & Credits
- This demo was prepared for presentation purposes. Feel free to adapt and extend it.

Contact
