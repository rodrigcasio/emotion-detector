# Emotion Detector (Flask & Python)

This is a web application I built as part of my IBM Full-Stack Developer certification course. It's an emotion detection app that analyzes text and identifies emotions using the Watson NLP API. This was my first time working with Flask, Python web development, and integrating AI/NLP services, and I put a lot of effort into understanding how to build web applications with Python.

## What does it do?

- **Emotion Analysis**: Takes text input from users and analyzes it to detect emotions (anger, disgust, fear, joy, sadness).
- **Web Interface**: A simple web page where users can enter text and see emotion analysis results.
- **API Integration**: Connects to IBM Watson NLP API to perform emotion detection.
- **Real-time Results**: Shows emotion scores and identifies the dominant emotion in the text.
- **Error Handling**: Handles invalid inputs and API errors gracefully.

## Features

- **Text Input**: Users can enter any text they want to analyze
- **Emotion Detection**: Analyzes text and returns scores for five emotions:
  - Anger
  - Disgust
  - Fear
  - Joy
  - Sadness
- **Dominant Emotion**: Identifies which emotion has the highest score
- **Web Interface**: Clean, simple interface built with Flask and Bootstrap
- **Unit Tests**: Includes test cases to verify emotion detection works correctly

## Why did I make this?

I built this as part of my IBM Full-Stack Developer course to learn about:
- Building web applications with Flask (Python web framework)
- Integrating third-party APIs (Watson NLP)
- Handling HTTP requests and responses
- Working with JSON data
- Creating user interfaces with HTML, CSS, and JavaScript
- Writing unit tests in Python

## Technologies Used

- **Python**: Core programming language
- **Flask**: Web framework for building the application
- **Watson NLP API**: IBM's natural language processing service for emotion detection
- **HTML/CSS/JavaScript**: For the web interface
- **Bootstrap**: For styling the web page
- **Requests**: For making HTTP requests to the Watson API
- **unittest**: For writing and running tests

## Important Note

⚠️ **The Watson NLP API is only accessible within the IBM Skills Network Theia Lab environment.** The API used in this project is hosted on the Skills Network platform, so the application needs to run in that environment to work properly.

## How to Run

1. Make sure you have Python 3 installed on your computer.
2. Create a virtual environment (recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
   (Note: The file is named `requirements.xt` - you may need to rename it to `requirements.txt` or install packages manually)
4. Run the Flask server:
   ```
   python server.py
   ```
5. Open your browser and visit `http://localhost:5000`

## Running Tests

To run the unit tests:
```
python test_emotion_detection.py
```

The tests verify that the emotion detector correctly identifies different emotions in sample text.

## Project Structure

- `server.py` - Main Flask application with routes and server setup
- `EmotionDetection/emotion_detection.py` - Function that connects to Watson NLP API
- `templates/index.html` - Web interface for the application
- `static/mywebscript.js` - JavaScript for handling user interactions
- `test_emotion_detection.py` - Unit tests for emotion detection
- `requirements.xt` - Python package dependencies

## Example Usage

1. Start the Flask server
2. Open the web page in your browser
3. Enter text like "I am glad this happened" or "I am really mad about this"
4. Click "Run Sentiment Analysis"
5. View the emotion scores and dominant emotion

## What I Learned

- How to build web applications with Flask
- Making HTTP requests to external APIs
- Parsing and working with JSON responses
- Error handling for API failures
- Creating user interfaces with HTML, CSS, and JavaScript
- Writing unit tests in Python
- Working with virtual environments and Python packages
- Understanding how AI/NLP services can be integrated into web apps

## Author

Rodrigo Casio  
[My GitHub Profile](https://github.com/rodrigcasio)
