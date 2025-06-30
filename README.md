# 🎮 React Quiz Game App

This is an interactive quiz application built using **React JS**. It allows users to test their knowledge with a series of multiple-choice questions. The app tracks progress, scores, highscore, and even includes a timer.

---

## ✨ Features

- 🔄 Fetches quiz questions from JSON data
- ✅ Real-time answer checking
- 🧠 Score + Highscore tracking
- 🕒 Timer (30 seconds per question)
- 📊 Progress bar
- 💯 Percentage-based emoji result
- 🔁 Restart quiz feature
- 🧪 Bonus: Date Counter (Reducer Practice)

---

## 🚀 Technologies Used

- React JS
- useReducer, useEffect Hooks
- HTML, CSS
- JSON (as database for questions)

---

## 🗂️ Folder Structure

```
react-quiz/
├── public/
│   └── index.html
├── src/
│   ├── App.js               # Main app with quiz logic
│   ├── index.js             # React root render
│   ├── index.css            # Styles
│   ├── components/
│   │   ├── DateCounter.js
│   │   ├── Error.js
│   │   ├── FinishScreen.js
│   │   ├── Footer.js
│   │   ├── Header.js
│   │   ├── Loader.js
│   │   ├── Main.js
│   │   ├── NextButton.js
│   │   ├── Options.js
│   │   ├── Progress.js
│   │   ├── Question.js
│   │   ├── StartScreen.js
│   │   └── Timer.js
│   └── data/
│       └── questions.json   # Quiz questions database
├── package.json
└── README.md
```

---

## 🖥️ How to Run the Project Locally

1. **Clone the repository**

   ```bash
   git clone https://github.com/ershamshad12/React-Quiz-Game.git
   cd react-quiz-app
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**

   ```bash
   npm start
   ```

4. Open in browser:  
   [http://localhost:3000](http://localhost:3000)

---

## 🧠 Quiz Data Format

Your quiz data is stored in `data/questions.json` and looks like this:

```json
{
  "questions": [
    {
      "question": "Which is the most popular JavaScript framework?",
      "options": ["Angular", "React", "Svelte", "Vue"],
      "correctOption": 1,
      "points": 10
    },
    {
      "question": "Which company invented React?",
      "options": ["Google", "Apple", "Netflix", "Facebook"],
      "correctOption": 3,
      "points": 10
    }
    // ...more questions
  ]
}
```

👉 The app fetches questions from this file using:

```js
fetch("http://localhost:3000/questions");
```

Make sure your `json-server` or dev server is properly serving the file at `/questions`.

---

## 📦 Components Overview

### `App.js`

- Handles all quiz states using `useReducer`
- Manages question flow, answer check, timer, finish, and restart

### `FinishScreen.js`

- Shows final score with percentage and emoji
- Displays highscore
- Option to restart quiz

### `Error.js` & `Loader.js`

- Display loading or error states while fetching data

### `Timer.js`

- Counts down from total available seconds
- Ends quiz when time runs out

### `DateCounter.js` _(Bonus)_

- Demo of `useReducer` to increment/decrement days from a fixed date

---

## ✨ Future Enhancements (Optional Ideas)

- Add categories for questions
- Save highscores in `localStorage`
- Add animations with Framer Motion
- Deploy to Netlify or Vercel

---

## 👤 Author

**Md Shamshad Ansari**  
🎓 CSE Graduate | 🚀 Java Full Stack Learner @ JSpiders  
📍 From Sitamarhi, Bihar | Currently in Delhi  
🔗 [https://github.com/ershamshad12/https://www.linkedin.com/in/md-shamshad-feb2002//]

---

## 📄 License

This project is licensed under the MIT License.

---
