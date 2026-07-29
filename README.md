# Penner Family Pages

Welcome to the Penner Family website! This site is currently serving as the central hub for **Baby Penner**, expected August 10, 2026. 

It features a live countdown, a professional dashboard of all friends and family predictions, and a hidden Retro Arcade scoreboard to crown the ultimate prediction winner once the baby is born.

## Project Structure

- `index.html` - The main landing page for the Penner Family site.
- `results.html` - The classy, professional dashboard displaying all predictions, aggregate charts, and a timeline of guesses.
- `scoreboard.html` - A hidden, retro-arcade themed leaderboard. It dynamically ranks all participants based on their guesses against the official baby stats.
- `admin.html` - A private, user-friendly tool to safely generate the JSON string when the baby arrives.
- `official_answers.json` - The database file that the scoreboard reads to determine the winner.

---

## How to Update the Scoreboard (When the Baby Arrives!)

To ensure there are no typos and the scoreboard works perfectly on the big day, follow this foolproof workflow:

1. **Open the Admin Tool**: Go to your live website and navigate to `/admin.html`.
2. **Check off the Stats**: Change *Is the baby born?* to **YES!**, and check off the baby's actual stats (Gender, Weight, Hair Color, etc.).
3. **Generate the Code**: Click the **"Generate Official Code"** button. The page will automatically write a perfectly formatted JSON block and copy it to your computer's clipboard.
4. **Update GitHub**: 
   - Log into this GitHub repository.
   - Open the `official_answers.json` file.
   - Click the pencil icon to edit.
   - Delete all the old text, and **paste** what is on your clipboard.
   - Click **"Commit changes"** to save.
5. **Celebrate**: Go back to your website and open the Arcade Leaderboard (`/scoreboard.html`). The page will instantly read the new JSON file, populate the "Official Baby Stats" box, grade everyone's predictions, and crown the winner!

## The Scoring System
The JavaScript engine automatically grades participants based on the following rules:
- **Gender Match**: 5,000 pts
- **Birth Date**: 10,000 pts *(penalty of -1,000 pts for every day off)*
- **Weight**: 5,000 pts *(penalty of -500 pts for every ounce off)*
- **Hair Color**: 2,000 pts
- **Hair Style**: 2,000 pts
- **Eye Color**: 2,000 pts
- **Jackpot (Name Picked)**: 10,000 pts bonus if the parents pick a name the participant suggested!
