# Quiz Game App

## Description

This is a **simple Quiz Game App** built with **ReactJS** as a final project for our class. The app allows users to take a fun quiz, track their score, and navigate between different pages. It’s designed to cover multiple functionalities while keeping things beginner-friendly.

The app includes **5 main pages/views** and demonstrates basic React concepts like components, state management, and routing.

---

## Features

* **Home Page**: Introduction and start button to begin the quiz.
* **Quiz Page**: Displays multiple-choice questions with options for the user to select.
* **Score Page**: Shows the user's total score at the end of the quiz.
* **About Page**: Information about the app and its creators.
* **Settings Page**: Allows users to reset the quiz or change simple settings (like theme or difficulty).

Other functionalities:

* Navigation between pages using React Router.
* Basic state management using `useState`.
* Conditional rendering to show different views based on user progress.

---

## Installation

1. Clone the repository:

   ```bash
   git clone <your-repo-url>
   ```
2. Navigate to the project folder:

   ```bash
   cd quiz-game-app
   ```
3. Install dependencies:

   ```bash
   npm install
   ```
4. Start the app:

   ```bash
   npm run dev
   ```

---

## Usage

1. Open the app in your browser.
2. Choose between categories of quizes.
3. Click **Start Quiz** on the Home Page.
4. Answer the multiple-choice questions on the Quiz Page.
5. View your score on the Score Page after finishing.
6. Use the navigation menu to check out more quizes currently available.

---

## Technologies

* ReactJS
* React Router
* TailwindCSS for styling
* `useState` and `useEffect` hooks

---

## Notes

* This is a beginner-level project.
* The quiz questions are hardcoded (no backend yet).
* The project demonstrates routing, component composition, and state management in React.

## Prerequisites

Before you run this project locally, make sure you have:

- Node.js (v18 recommended). You can check your Node version with `node --version`.
- npm (bundled with Node) — check with `npm --version`.
- Git to clone and manage the repository.

This project uses Vite as the dev server. The correct command to start the app in development is `npm run dev` (not `npm start`).

## Teammates guide — quick setup

1. Clone the repo and switch to the working branch:

   git clone < your-repo-url >
   
   cd inf-651-quiz-game-app

2. Install dependencies:

   npm install

3. Start the development server (open http://localhost:5173 by default):

   npm run dev


Notes:

- Vite typically serves the dev app on port 5173. If `http://localhost:3000` is mentioned elsewhere, prefer the terminal output from `npm run dev` to know the exact URL.
- If you run into issues installing dependencies, removing `node_modules` and reinstalling (`rm -rf node_modules package-lock.json && npm install`) often helps.

## Contributing / Workflow tips

The project uses a small branching workflow so demos and tests can run on a shared branch before changes reach `master`.

Guidelines:

- Start from the `master` branch and make sure it is up to date:

   ```bash
   git checkout master
   git pull
   ```

- Create a branch named for your work (examples: `feat/add-question`, `fix/button-style`):

   ```bash
   git fetch origin
   git checkout < your branch >
   ```

- Commit locally with clear messages and push the branch to the remote:

   ```bash
   git add .
   git commit -m "feat: add question component"
   git push 
   ```

- Open a Pull Request targeting the `demo` branch (not `master`) so the team can test the change in the demo environment. Include a short description, testing steps, and any screenshots.


- After the change is tested on `demo` and everything works, the `demo` branch will be merged into `master` (typically by whoever manages releases). If you are responsible for merging, create a PR from `demo` to `master` and follow the repo's merge process.

Notes:

- Keep PRs focused and small where possible — it's easier to review and test.
- If you need help reproducing an issue locally, include steps and terminal output in the PR comments.

## Troubleshooting

- If the dev server fails to start, check for another process using the port and consult the terminal for the error.
- If React or Vite reports incompatible versions, confirm your Node version and installed package versions from `package.json`.
- When in doubt, share the terminal output with the team — it usually contains the error and suggested fixes.
