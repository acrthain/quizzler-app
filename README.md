# Quizzler

A desktop true/false trivia quiz app built with Python and Tkinter, pulling live questions from the Open Trivia Database API.

## What it does

- Fetches a fresh set of computer science true/false questions from the Open Trivia Database on each run
- Displays one question at a time in a simple graphical interface
- Gives instant visual feedback (green for correct, red for incorrect) when you answer
- Tracks and displays your score as you go, and shows a completion message at the end

## How it works

- **`main.py`** — fetches question data, builds the question bank, and starts the quiz
- **`data.py`** — handles the API request to Open Trivia Database and returns the raw question data
- **`question_model.py`** — defines the `Question` class, representing a single question and its answer
- **`quiz_brain.py`** — defines the `QuizBrain` class, which tracks quiz progress, current question, and score, and checks submitted answers
- **`ui.py`** — defines the `QuizInterface` class, building the Tkinter GUI and handling user interaction

## Tech used

- Python 3
- Tkinter (GUI)
- `requests` (API calls)
- Open Trivia Database API (external data source, no API key required)
- Object-oriented design (separate classes for questions, quiz logic, and interface)

## What I'd improve next

- Let the user choose question category and difficulty before starting
- Add a local fallback question set for when the API is unavailable
- Show a summary screen with which questions were answered incorrectly

## Background

Built as part of a 100 Days of Code Python bootcamp, while working toward a software engineering internship.
