## Interactive Quiz-App
Welcome to Interactive Quiz-App, an interactive quiz app that challenges your knowledge across various categories and difficulty levels.

## Project Overview
This project consists of the following key files:
- `index.html`: The HTML file that defines the structure of the web page.
- `style.css`: The CSS file that styles the elements on the page.
- `script.js`: The JavaScript file that handles the quiz logic and interactions.
- `countdown.mp3`: A short audio file used for countdown effects.

## API Usage
Interactive Quiz-App fetches quiz questions from the Open Trivia Database API (https://opentdb.com/api.php). The `startQuiz` function in `script.js` constructs a URL based on user-selected options (number of questions, category, difficulty) and makes a GET request to the API. The questions are then dynamically loaded into the quiz.
```javascript
// API request URL construction
const url = `https://opentdb.com/api.php?amount=${num}&category=${cat}&difficulty=${diff}&type=multiple`;
