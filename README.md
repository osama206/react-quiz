# React Quiz Application

This project is a React application designed to provide an interactive quiz experience. Users can start the quiz, answer questions, and see their progress and final score. The application demonstrates the use of React components, state management, and conditional rendering.

## Features

- **Loading Screen**: Displays a loading spinner while questions are being fetched.
- **Error Handling**: Shows an error message if there's an issue fetching questions.
- **Start Screen**: Welcomes users and allows them to start the quiz.
- **Question Display**: Presents each quiz question and its multiple-choice options.
- **Progress Tracking**: Shows current progress through a progress bar and score display.
- **Timer**: Counts down the time remaining for the quiz.
- **Navigation**: Provides buttons to move to the next question or finish the quiz.
- **Finish Screen**: Displays the final score, high score, and a restart button.
- **Date Counter**: An additional component that allows users to increment or decrement a date based on a counter and step value.

## Components

- **App**: The main component that orchestrates the quiz flow.
- **Header**: Displays the quiz title and logo.
- **Main**: Wrapper component for the main content.
- **Loader**: Shows a loading spinner.
- **Error**: Displays an error message.
- **StartScreen**: Welcomes users and starts the quiz.
- **Question**: Displays the current question and options.
- **Options**: Renders answer options and handles answer selection.
- **NextButton**: Provides navigation between questions.
- **Progress**: Displays quiz progress and score.
- **FinishScreen**: Shows final results and high score.
- **Footer**: Wraps footer content like the timer and navigation buttons.
- **Timer**: Displays a countdown timer.
- **DateCounter**: A separate counter component that uses `useReducer` to manage state, adjusting a date based on count and step values.

## State Management

The quiz state is managed using a custom context (`useQuiz`) that provides a global state and dispatch function. The state includes:
- `status`: Current quiz status (loading, ready, active, finished).
- `questions`: Array of quiz questions.
- `index`: Index of the current question.
- `points`: Current score.
- `maxPossiblePoints`: Maximum possible score.
- `highscore`: High score.
- `secondsRemaining`: Time remaining.
- `answer`: Current answer to the question.

## Example Questions

The example questions cover basic React concepts such as components, state, props, hooks, and lifecycle methods. Each question has multiple options and points associated with it.

## Running the Project

To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/osama206/react-quiz.git
   ```
2. **Navigate to the project directory**:
   ```bash
   cd react-quiz
   ```
3. **Install dependencies**
   ```bash
   npm install
   ```
4. **Start the development server**:
   ```bash
   npm start
   ```
5. Open your browser and go to `http://localhost:3000` to see the application in action.
