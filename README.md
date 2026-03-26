# TableTalk Narrative Voice Processing System

##  Overview
This project implements an AI-based system for processing, analyzing, and retrieving narrative voice recordings used in storytelling environments such as tabletop games.

The system performs audio feature extraction, emotion classification, speech-to-text transcription, and query-based audio retrieval.


##  Features

### Task 1: Audio Processing
- Loaded and normalized audio recordings
- Extracted features:
  - MFCC (13 coefficients)
  - Pitch
  - Energy (RMS)
  - Spectral Centroid
  - Duration
- Output stored in `features.csv`



###  Task 2: Narrative Tone Classification
- Trained a Random Forest classifier
- Input: extracted audio features
- Output: emotion labels (calm, happy, angry, etc.)
- Achieved ~60% accuracy



###  Task 3: Speech-to-Text Transcription
- Used OpenAI Whisper model
- Transcribed multiple audio recordings
- Output stored in `transcriptions.csv`



###  Task 4: Narrative Audio Retrieval
- Implemented query-based filtering system
- Supports queries such as:
  - Calm narration
  - High-energy speech
  - Angry dialogue
- Retrieves matching audio recordings using features



###  Storytelling Audio Analysis
- Analyzed differences between storytelling narration and conversational speech
- Key features:
  - Pitch variation
  - Energy dynamics
  - Pacing and pauses
  - Sentence structure



##  Project Structure
│
├── TableTalk_Project.ipynb # Main notebook (all tasks)
|
├── features.csv # Extracted audio features
├── transcriptions.csv # Speech-to-text outputs
├── README.md # Project documentation



##  How to Run

1. Open the notebook:

TableTalk_Project.ipynb


2. Install required libraries:

pip install librosa numpy pandas scikit-learn openai-whisper


3. Upload dataset (RAVDESS or any .wav files)

4. Run all cells sequentially:
- Task 1 → Feature extraction
- Task 2 → Model training
- Task 3 → Transcription
- Task 4 → Retrieval



##  Outputs

- `features.csv` → structured dataset for ML
- `transcriptions.csv` → generated speech transcripts
- Model accuracy and retrieval results displayed in notebook



## Technologies Used

- Python
- librosa
- numpy
- pandas
- scikit-learn
- OpenAI Whisper



##  Dataset

RAVDESS Emotional Speech Dataset 

---

## Conclusion

This project demonstrates a complete pipeline for processing, analyzing, and retrieving narrative audio recordings. It combines signal processing, machine learning, and speech recognition to support storytelling applications.
