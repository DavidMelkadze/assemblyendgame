🎮 Assembly: Endgame — React
A fun word-guessing game built with React that challenges you to reveal a hidden word. Programming languages fall as you make wrong guesses — guess incorrectly 8 times and it's game over. Includes responsive design for all screen sizes, confetti celebrations, and dynamic farewell messages.

🚀 Live Demo
Deploy to Vercel or Netlify to share your game!

🧭 Quick Features
Guess letters by clicking the keyboard
Correct guesses reveal letters in the word
Wrong guesses eliminate programming languages from the board
8 attempts to guess the word — each wrong guess counts down
Win and celebrate with confetti 🎉
Lose and get a funny farewell message
Responsive layout: works great on mobile and desktop
Keyboard buttons disable once the game ends
Play again with the "New Game" button
Accessible UI with aria-live status updates
⚡ How to Use
Start the app — a secret word appears with empty tiles
Click any letter from the keyboard to make a guess
If the letter is in the word, it'll be revealed
If not, a programming language chip gets marked as lost (☠️)
Keep guessing until you either:
Win: reveal all letters before running out of attempts
Lose: eliminate all 8 programming languages
Click "New Game" to play again
📂 Project Structure (Key Files)

| File | Purpose |
|------|---------|
| App.jsx | Game logic, state tracking, win/loss detection |
| index.css | Responsive styling, media queries for mobile/desktop |
| languages.js | Language chip data with colors and themes |
| utils.js | Random word selection, farewell text generator |
| words.js | Word bank (500+ words to guess) |
🛠️ Tech Stack
React 19 (functional components + hooks)
JavaScript (ES6+)
CSS (custom properties, responsive design)
Vite (dev server / build tool)
clsx (conditional class names)
react-confetti (celebration effect on win)

📝 What I Learned
Managing complex game state with multiple useState hooks
Determining win/loss conditions through state calculations
Rendering dynamic UI elements based on game progress
Conditional styling with CSS classes and inline styles
Responsive design with mobile-first media queries
Accessibility best practices (aria-live, aria-label, semantic HTML)
Using modular data files for business logic separation
Confetti animations for user delight and feedback

⚙ Decisions & Notes
The game tracks guessedLetters as an array and derives all game state from it (currentWord, wrongGuessCount, isGameWon, isGameLost).
Language chips are stored as objects with name, backgroundColor, and color for easy theming.
The keyboard is dynamically generated from the alphabet string and mapped to button elements.
Farewell messages are randomly selected when a wrong guess occurs — adds personality to losses.
Mobile breakpoint at 640px uses smaller tiles and buttons; tablet/desktop at 768px+ scales everything up.
Missing letters on game loss are highlighted in red (#ec5d49) to show what the player missed.

🌟 Possible Future Improvements
Add difficulty levels (easy, medium, hard) with different word pools
Include category hints or word descriptions before guessing
Track stats: wins, losses, accuracy percentage
Add a leaderboard or high score display
Implement multiplayer guessing (turn-based)
Add sound effects for correct/wrong guesses
Create a "Daily Challenge" mode with the same word each day
Add animations for letter reveals and language chip eliminations
Include a timer for speed-run mode
Persist stats to localStorage
Write unit tests for game logic (Jest + React Testing Library)
Add keyboard support to detect physical key presses (not just clicks)

♿ Accessibility
All buttons have aria-label attributes for screen readers
Game status uses aria-live="polite" to announce wins/losses
Disabled buttons show cursor: not-allowed and reduced opacity
Keyboard buttons correctly show disabled state via aria-disabled
Screen-reader only section provides current word progress and attempt count

🙏 Acknowledgements
Built as a learning and portfolio project to practice React state management, game logic, and responsive design.

👨‍💻 Author
Adam — Frontend Developer in progress 🚀
Focused on building interactive React apps with clean code and great UX
