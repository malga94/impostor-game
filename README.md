# The Impostor Game

A simple web-based party game where players try to identify the impostor(s) among them.

## How to Play

1. Players take turns looking at the screen privately
2. Most players (Actors) see a word - they must describe it without saying it
3. The Impostor(s) don't see the word - they must blend in and guess what it is
4. After everyone has seen their role, discuss and try to find the impostor(s)!

## Running the Game

The game needs to be served via HTTP (not opened directly as a file) to load the word lists.

### Using Python (recommended)

Navigate to the project directory and run:

```bash
python3 -m http.server 8000
```

Then open your browser to: **http://localhost:8000**

### Alternative: Using Node.js

If you have Node.js installed:

```bash
npx http-server -p 8000
```

Then open: **http://localhost:8000**

### Alternative: Using PHP

```bash
php -S localhost:8000
```

Then open: **http://localhost:8000**

## Features

- Dynamic player management (add/remove players)
- Configurable number of impostors
- Multi-language support (English and Italian)
- Responsive design for mobile devices
- Sequential private role reveal system

## Adding More Words

Edit the CSV files to add more words:
- `words_english.csv` - English words
- `words_italian.csv` - Italian words

Add one word per line in each file.

## Files

- `index.html` - Main game file
- `words_english.csv` - English word list
- `words_italian.csv` - Italian word list
- `README.md` - This file
