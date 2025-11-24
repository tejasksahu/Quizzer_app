# Quizzer_app
Quizzer is a, GUI-based quiz application built with Python. It fetches real-time "True/False" trivia questions from the Open Trivia Database API and presents them in an interactive Tkinter interface.

Features
Fresh Content:   Requests 10 new random questions every time the app is launched from the Open Trivia DB API.
Interactive GUI: Built with Tkinter, featuring a responsive canvas that changes color to provide immediate feedback (Green for correct, Red for incorrect).
Score Tracking:  Keeps track of the user's score in real-time.

Project Structure
main.py:           The entry point of the application. Set up the flow b etween data, the quiz model, and the UI.
ui.py:             Handles the Tkinter Graphical User Interface, including the window, canvas, buttons, and event loop.
quiz_brain.py:     Contains the QuizBrain class which manages the game state (score, question number, checking answers).
data.py:           Handles the API connection to opentdb.com to fetch question data.
question_model.py: Defines the Question class to structure API data into objects.

Prerequisites
Python 3.x
The "requests" library

Installation & Setup
Clone the repository:
git clone [https://github.com/yourusername/Quizzer-app.git](https://github.com/yourusername/Quizzer-app.git)cd Quizzer-app

Install dependencies:
pip install requests

Asset Requirement:
Ensure you have an images folder in the root directory containing:
true.png (Checkmark icon)
false.png (Cross icon)

Usage
Run the file main.py
Read the question displayed on the card.
Press the Green Check button for "True" or the Red X button for "False".
The screen will flash Green (Correct) or Red (Wrong).
Try to get a perfect 10/10 score!

API Reference
This project uses the Open Trivia DB API.
Endpoint: https://opentdb.com/api.php
Parameters used: amount=10, type=boolean
