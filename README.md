## Interactive Quiz-App
Welcome to Interactive Quiz-App, an interactive quiz app that challenges your knowledge across various categories and difficulty levels.

## Project Overview
This project consists of the following key files:
- `index.html`: The HTML file that defines the structure of the web page.
- `style.css`: The CSS file that styles the elements on the page.
- `script.js`: The JavaScript file that handles the quiz logic and interactions.
- `countdown.mp3`: A short audio file used for countdown effects.

## Features
- **Dynamic Question Rendering:** Questions are fetched from the API and dynamically rendered on the page using JavaScript.
- **Countdown Timer:** A timer is implemented for each question, providing a time limit for answers.
- **Answer Feedback:** Users receive instant feedback on the correctness of their answers.
- **Score Tracking:** The app keeps track of the user's score throughout the quiz.
- **Category and Difficulty Selection:** Users can customize their quiz experience by selecting the number of questions, category, and difficulty.

## How to Use
1. Clone this repository to your local machine.
   ```bash
    git clone https://github.com/vasanthsai14/quiz-app-javascript.git
    ``` 
2. Open index.html in your web browser to launch the quiz app.
3. Customize your quiz experience by selecting the number of questions, category, and difficulty.
4. Click "Start Quiz" to begin the quiz and test your knowledge.

## API Usage
Interactive Quiz-App fetches quiz questions from the Open Trivia Database API (https://opentdb.com/api.php). The `startQuiz` function in `script.js` constructs a URL based on user-selected options (number of questions, category, difficulty) and makes a GET request to the API. The questions are then dynamically loaded into the quiz.
```javascript
// API request URL construction
const url = `https://opentdb.com/api.php?amount=${num}&category=${cat}&difficulty=${diff}&type=multiple`;
