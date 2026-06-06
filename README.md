# 🤖 JASMINE AI – Terminal-Based Voice Assistant

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue.svg">
  <img src="https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange.svg">
  <img src="https://img.shields.io/badge/NLP-Intent%20Classification-green.svg">
  <img src="https://img.shields.io/badge/Status-Working-success.svg">
</p>

## 📌 Overview

JASMINE AI is a Machine Learning-powered terminal-based voice assistant . The assistant listens to voice commands, converts speech into text, predicts user intent using a trained TensorFlow neural network, and executes real-world tasks such as opening applications, searching the web, controlling system settings, retrieving information from Wikipedia, reporting weather updates, taking notes, and more.

Unlike rule-based chatbots that rely solely on if-else conditions, JASMINE AI uses Natural Language Processing (NLP) and Intent Classification to understand user requests and provide intelligent responses.

---

# 🎯 Features

### 🗣️ Voice Interaction

* Speech-to-Text using Google Speech Recognition
* Text-to-Speech using Pyttsx3
* Real-time voice command processing
* Natural conversational responses

### 🧠 Machine Learning & NLP

* Custom intent classification model
* TensorFlow/Keras neural network
* Tokenization and text preprocessing
* Confidence-based intent prediction
* Label encoding for intent mapping

### 💻 System Automation

* Open Chrome browser
* Open Notepad
* Open Calculator
* Open Command Prompt


### 🌐 Internet Utilities

* Google Search
* YouTube Search
* Wikipedia Summaries
* Latest News Access
* Weather Reports

### 🔊 Media Controls

* Increase Volume
* Decrease Volume
* Mute Volume
* Close Browser Tabs

### 📝 Productivity Tools

* Voice Notes
* Reminders




# 🏗️ Project Architecture

```text
User Voice
     │
     ▼
Speech Recognition
     │
     ▼
Text Command
     │
     ▼
Tokenizer
     │
     ▼
Neural Network Model
     │
     ▼
Intent Prediction
     │
     ▼
Command Execution
     │
     ▼
Text Response
     │
     ▼
Speech Output
```

---

# 📂 Project Structure

```text
Jasmine-AI-Voice-Assistant/
│
├── main.py
├── model_train.py
├── intents.json
├── requirements.txt
│
├── chat_model.h5
├── tokenizer.pkl
├── label_encoder.pkl
│
└── README.md
```

---

# 📁 File Explanation

## 1️⃣ intents.json

The knowledge base of the assistant.

Contains:

* Intent Tags
* User Patterns
* Assistant Responses

Example:

```json
{
  "tag": "greeting",
  "patterns": [
    "hello",
    "hi",
    "hey jasmine"
  ],
  "responses": [
    "Hello Boss!"
  ]
}
```

---

## 2️⃣ model_train.py

Responsible for training the Machine Learning model.

### Tasks Performed

* Load intents dataset
* Extract patterns and labels
* Tokenize sentences
* Encode labels
* Create neural network
* Train model
* Save trained files

Generated files:

```text
chat_model.h5
tokenizer.pkl
label_encoder.pkl
```

---

## 3️⃣ main.py

Main application file.

Responsibilities:

* Listen to voice commands
* Predict user intent
* Generate responses
* Execute actions
* Speak output

---

## 4️⃣ requirements.txt

Contains all project dependencies.

---

# 🔥 Machine Learning Workflow

## Step 1: Create Custom Dataset

All conversations are stored inside:

```text
intents.json
```

Example categories:

* Greeting
* Goodbye
* Weather
* Search
* Open Applications
* Wikipedia
* Notes
* News

---

## Step 2: Text Processing

Tokenizer converts text into numerical sequences.

Example:

```text
open calculator
```

becomes

```text
[8, 20]
```

---

## Step 3: Label Encoding

Intent names:

```text
greeting
weather
open_app
```

become

```text
0
1
2
```

---

## Step 4: Neural Network Training

Architecture:

```text
Embedding Layer
       ↓
Global Average Pooling
       ↓
Dense Layer (ReLU)
       ↓
Dense Layer (ReLU)
       ↓
Softmax Output
```

---

## Step 5: Save AI Components

### chat_model.h5

Stores trained neural network weights.

### tokenizer.pkl

Stores learned vocabulary.

### label_encoder.pkl

Stores intent-label mappings.

---

# 🎙️ Speech Recognition

Implemented using:

```python
SpeechRecognition
```

Process:

```text
Microphone
    ↓
Audio Input
    ↓
Google Speech Recognition
    ↓
Text Output
```

Example:

```text
"Open Calculator"
```

↓

```text
open calculator
```

---

# 🔊 Text-to-Speech

Implemented using:

```python
pyttsx3
```

Capabilities:

* Offline voice synthesis
* Adjustable speaking rate
* Multiple voice profiles

Example:

```python
speak("Hello Boss")
```

---

# ⚡ Supported Commands

## General Conversation

```text
Hello
Who are you
Who created you
Thank you
Goodbye
```

---

## Search Commands

```text
Search for Python tutorials
Google Artificial Intelligence
```

---

## YouTube Commands

```text
Play Believer on YouTube
Search music on YouTube
```

---

## Application Commands

```text
Open Notepad
Open Calculator
Open Chrome

```

---

## Information Commands

```text
What is the time
Tell me the date
What is the weather
Who is Elon Musk
Tell me about India
```

---

## Media Commands

```text
Volume Up
Volume Down
Mute
Unmute
Close Tab
```

---

## Productivity Commands

```text
Take a note
Set reminder
```

---

# 🚀 Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/Jasmine-AI-Voice-Assistant.git
cd Jasmine-AI-Voice-Assistant
```

## Create Virtual Environment

```bash
python -m venv venv
```

Activate:

```bash
venv\Scripts\activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🧠 Train the Model

```bash
python model_train.py
```

This generates:

```text
chat_model.h5
tokenizer.pkl
label_encoder.pkl
```

---

# ▶️ Run JASMINE AI

```bash
python main.py
```

Expected Output:

```text
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🤖 JASMINE AI ASSISTANT ONLINE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Hello Boss, Jasmine is online and fully operational.
```

---

# 🛠️ Tech Stack

### Programming Language

* Python

### Machine Learning

* TensorFlow
* Keras
* NumPy
* Scikit-Learn

### NLP

* Tokenization
* Intent Classification
* Label Encoding

### Speech Processing

* SpeechRecognition
* PyAudio
* pyttsx3

### Automation

* PyAutoGUI
* OS Commands

### APIs

* Wikipedia API
* WTTR Weather API
* Google Search

---


