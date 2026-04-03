# 🎮 **Assembly: Endgame — React**

A **fun, interactive word-guessing game** inspired by Hangman, built with **React** as a **portfolio project**.
Guess the hidden word before running out of attempts — each wrong guess eliminates a programming language from the board.

> ⚠️ Originally inspired by a Scrimba project — extended and customized with additional features and improvements.

---

## 🚀 **Live Demo**

**https://assemblyendgame-pi.vercel.app/**

---

## 🧭 **Quick Features**

* Guess letters using an interactive on-screen keyboard
* Correct guesses reveal letters in the word
* Wrong guesses eliminate programming languages 💀
* 8 attempts total — game ends when attempts run out
* Win state with **confetti celebration 🎉**
* Lose state with dynamic farewell messages
* Fully **responsive design** (mobile → desktop)
* Keyboard buttons disable after game ends
* “New Game” button to restart instantly
* Accessible UI with `aria-live` updates

---

## ⚡ **How to Use**

1. Start the game — a hidden word appears.
2. Click letters from the keyboard to guess.
3. If the letter exists → it gets revealed.
4. If not → a programming language is eliminated.
5. Keep guessing until:

   * **Win** → reveal the full word
   * **Lose** → all 8 attempts are used
6. Click **New Game** to play again.

---

## 📂 **Project Structure (Key Files)**

| File           | Purpose                                    |
| -------------- | ------------------------------------------ |
| `App.jsx`      | Main game logic, state, win/loss detection |
| `index.css`    | Styling + responsive layout                |
| `languages.js` | Programming language data (UI + colors)    |
| `utils.js`     | Helper functions (random word, messages)   |
| `words.js`     | Word bank (500+ words)                     |

---

## 🛠️ **Tech Stack**

* **React** (functional components + hooks)
* **JavaScript (ES6+)**
* **CSS** (responsive design, custom styling)
* **Vite** (build tool)
* **clsx** (conditional class names)
* **react-confetti** (win animation)

---

## 🚀 **My Improvements**

* Added **responsive design** for mobile, tablet, and desktop
* Improved overall **UI layout and styling**
* Cleaned and structured code for better readability

---

## 📝 **What I Learned**

* Managing **complex game state** with React hooks
* Deriving game logic (win/loss) from state
* Rendering dynamic UI based on user input
* Conditional styling using classes and state
* Building responsive layouts (mobile-first)
* Improving accessibility with ARIA attributes
* Separating logic into reusable modules
* Adding small UX details (animations, feedback)

---

## ⚙ **Decisions & Notes**

* Game state is derived from a single `guessedLetters` array
* Word, attempts, and results are calculated dynamically
* Language chips are stored as objects for flexible styling
* Keyboard is generated programmatically from alphabet
* Farewell messages are randomized for better UX
* Loss state highlights missing letters in red
* Responsive breakpoints ensure smooth scaling across devices

---

## 🌟 **Possible Future Improvements**

* Add difficulty levels (easy / medium / hard)
* Add hints or word categories
* Track player stats (wins, accuracy)
* Add leaderboard or scoring system
* Implement daily challenge mode
* Add animations for letter reveals
* Include sound effects
* Add keyboard input support
* Persist data with localStorage
* Write unit tests (Jest + React Testing Library)

---

## ♿ **Accessibility**

* Buttons include `aria-label` attributes
* Game status uses `aria-live` for announcements
* Disabled buttons clearly indicate state
* Screen-reader support for word progress

---

## 🙏 **Acknowledgements**

Based on a project from a Scrimba React course.
I independently implemented the logic, improved the UI, added responsiveness, and enhanced the overall user experience.

---

## 👨‍💻 **Author**

**David** — Frontend Developer in progress 🚀
Focused on building clean, interactive React apps
