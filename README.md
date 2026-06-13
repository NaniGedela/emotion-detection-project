# emotion-detection-project

# Emotion Detection Application using Watson NLP

## Project Overview

This project is an Emotion Detection web application built using the IBM Watson NLP library and Flask. The application analyzes user-provided text and detects the emotions expressed in it, including anger, disgust, fear, joy, and sadness. It also identifies the dominant emotion from the analysis.

## Features

* Detects emotions from text input.
* Identifies the dominant emotion.
* Provides a simple web-based interface using Flask.
* Includes unit tests to validate functionality.
* Handles invalid or blank user input gracefully.
* Passes static code analysis using Pylint.

## Project Structure

```text
EmotionDetection/
│
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
│
├── templates/
│   └── index.html
│
├── static/
│
├── test_emotion_detection.py
├── server.py
├── requirements.txt
└── README.md
```

## Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/EmotionDetection.git
cd EmotionDetection
```

### Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows**

```bash
venv\Scripts\activate
```

**Linux/macOS**

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Running the Application

Start the Flask server:

```bash
python server.py
```

Open your browser and navigate to:

```text
http://localhost:5000
```

## Example Output

Input:

```text
I am very happy today.
```

Output:

```python
{
    'anger': 0.01,
    'disgust': 0.01,
    'fear': 0.01,
    'joy': 0.95,
    'sadness': 0.02,
    'dominant_emotion': 'joy'
}
```

## Running Unit Tests

Execute:

```bash
python -m unittest test_emotion_detection.py
```

Expected result:

```text
.....
----------------------------------------------------------------------
Ran 5 tests

OK
```

## Static Code Analysis

Run:

```bash
pylint server.py
```

Expected result:

```text
Your code has been rated at 10.00/10
```

## Technologies Used

* Python
* Flask
* IBM Watson NLP
* Requests
* Unittest
* Pylint

## Author

Developed as part of the IBM Skills Network / Coursera project on Emotion Detection using Watson NLP.
