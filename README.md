# Three Clues

A browser word-guessing game about technical terms. Each round gives you three clues for a hidden term from operating systems, databases, computer networks, machine learning, security and more.

## How to play

- Read clue 1 and type your guess.
- Clue 2 unlocks after 2 attempts, and clue 3 after 4 attempts.
- After 5 attempts, a popup asks whether you want to reveal the answer or keep trying.
- After 10 attempts, a Reveal Answer button appears on screen.
- Terms never repeat until you have seen all of them. The "Terms asked" counter shows your progress.

## Run it

No install and no build step. Open `index.html` in any browser, or use the Live Server extension in VS Code.

## Customize

Open `index.html` and look for these lines in the script:

- `const WORDS = [ ... ]` holds the terms. Add one with `{ w: "MUTEX", cat: "Operating Systems", c: ["Clue 1", "Clue 2", "Clue 3"] },`.
- `const CLUE_UNLOCK = [0, 2, 4];` controls when each clue unlocks.
- `const POPUP_AT = 5;` and `const REVEAL_AT = 10;` control the reveal popup and the reveal button.

## Tech

Plain HTML, CSS and JavaScript in a single file. Progress is stored in the browser's localStorage.
