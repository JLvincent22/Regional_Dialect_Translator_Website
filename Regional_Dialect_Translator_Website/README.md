# Regional Dialect Translator

A static website based on the uploaded regional phrasebook PDF.

## Run locally
Open `index.html` in a browser. For microphone access, run it from localhost or HTTPS (for example, use VS Code Live Server); browsers usually block microphone access on ordinary local files.

## Deploy to Vercel
1. Push this folder to a GitHub repository.
2. In Vercel, choose **Add New → Project** and import the repository.
3. Keep Framework Preset as **Other**.
4. Leave Build Command and Output Directory empty (or set Output Directory to `.`).
5. Deploy. `index.html` is the entry page.

## Features
- English/Tagalog phrase lookup against the supplied PDF phrase list
- Region/dialect selector, including separate BARMM dialect choices
- Browser speech-to-text microphone input (Web Speech API; Chrome/Edge support varies)
- Text-to-speech result playback, copy, and clear
- Collapsible verified phrasebook cards with a decorative woven-inspired border

## Accuracy note
This is a phrasebook lookup, not an unrestricted machine translator. Only phrases included in the uploaded PDF are translated. The PDF does not provide every possible sentence for every region, so unsupported phrases are reported as not found rather than guessed.
