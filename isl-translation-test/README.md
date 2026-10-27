# Indian Sign Language Translator

An AI-powered application that recognizes Indian Sign Language (ISL) using a webcam and converts signs into English sentences.

## Features
- Recognizes 60 ISL signs.
- Uses MediaPipe to detect hand and body movements.
- Uses a BiLSTM model to recognize signs.
- Uses an LLM to convert recognized signs into grammatical English sentences.
- Supports sample videos and webcam input.

## How It Works
1. Captures hand and body movements.
2. Extracts landmarks from the video.
3. Recognizes signs using a trained deep learning model.
4. Converts the recognized signs into English sentences.

## Technologies Used
- Python
- PyTorch
- MediaPipe
- BiLSTM with Attention
- HTML, CSS and JavaScript
- LLM API

## Installation

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cpu
```

Create a `.env` file using `.env.example` and add your LLM API key.

## Run the Project

```bash
python -m server
```

Open `http://localhost:8000` in your browser.

## Dataset
The model is trained using the [INCLUDE Indian Sign Language Dataset](https://zenodo.org/records/4010759).

## Limitations
- Currently supports 60 signs.
- Recognition accuracy may vary with lighting and different signers.
- Continuous signing and facial expressions are not fully supported.

## Future Improvements
- Add more ISL signs.
- Improve continuous sign recognition.
- Support facial expressions and real-time sentence translation.
