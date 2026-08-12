# emotion-detection-project
emotion detection project IBM watson
Watson NLP Emotion Detection Web Application
Completed implementation of the IBM Embedded AI practice project using Watson NLP and Flask.
Features
Watson NLP emotion classification
Five emotion scores: anger, disgust, fear, joy, sadness
Dominant emotion calculation
Flask web UI
GET and POST emotion API
Input validation and error handling
Health endpoint
Pytest unit tests
Static-analysis-ready Python code
Run locally
```bash
python -m venv .venv
# Windows: .venv\\Scripts\\activate
# Linux/macOS: source .venv/bin/activate
pip install -r requirements.txt
python server.py
```
Open `http://127.0.0.1:5000`.
API
`GET /emotionDetector?textToAnalyze=I%20am%20happy`
`POST /emotionDetector` with JSON body:
```json
{"text":"I am happy today"}
```
`GET /health`
Tests
```bash
pytest -q
```
Static analysis
If Flake8 is installed:
```bash
flake8 .
```
The Watson NLP model is downloaded/loaded on first use and cached for subsequent requests.
