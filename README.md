# TableTalk_GSoc_2026
The TableTalk project aims to build a system that organizes and retrieves narrative voice recordings used in interactive storytelling environments such as tabletop role-playing games. These recordings may include narration, character dialogue, environmental descriptions, or dramatic moments that are triggered during gameplay.
# TableTalk Narrative Voice Processing

## Task 1: Audio Processing Pipeline

This project processes speech recordings and extracts meaningful audio features for machine learning.

### Features Extracted
- MFCC (13 coefficients)
- Pitch
- Energy (RMS)
- Spectral Centroid
- Duration

### Dataset
RAVDESS Emotional Speech Dataset (subset used)

### Output
A structured dataset (`features.csv`) containing extracted features for each audio file.

### Tools Used
- Python
- librosa
- numpy
- pandas
