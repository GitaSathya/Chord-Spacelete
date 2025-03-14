# Deep Learning-Based Audio Analysis and Chord Recognition System  
**Analyze custom audio files, generate chord music symbols, and visualize audio features using deep learning techniques.**

## Table of Contents
- [Project Overview](#project-overview)  
- [Features](#features)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Dependencies](#dependencies)  
- [Code Workflow](#code-workflow)  
- [Project Structure](#project-structure)  
- [Sample Results](#sample-results)  
- [Future Enhancements](#future-enhancements)  

---

## Project Overview  
This project focuses on **audio analysis and chord recognition** using deep learning. The code processes an **audio file (WAV format)**, extracts its features, and predicts corresponding chord music symbols. It also provides **visualizations** of the audio waveform, spectrogram, and predicted chords.

The model supports custom audio input, making it flexible for analyzing different types of audio files.

---

## Features  
- **Custom Audio Support**: Upload and analyze any WAV file.  
- **Chord Recognition**: Detect and display chord music symbols.  
- **Audio Visualization**: Generate visual representations such as waveform and spectrograms.  
- **Feature Extraction**: Use audio features like MFCCs, chroma, and spectral contrast for deep learning analysis.  

---

## Installation  

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/GitaSathya/Chord-Spacelete.git
   cd Chord-Spacelete
   ```

2. **Install Required Libraries**  
   Make sure you have Python installed. Install the dependencies:  
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage  

1. **Run the Script**  
   ```bash
   python VoicePitchDetection.ipynb
   ```

2. **Provide the Path to Your Custom Audio File**  
   The script will prompt you to enter the path of the audio file:  
   Example: `data/my_audio.wav`  

3. **View Results**  
   - Visualize the waveform and spectrogram.  
   - Predicted chord symbols will be displayed in the console.  

---

## Dependencies  
- **Python 3.8+**  
- **Librosa**: For audio analysis and feature extraction.  
- **NumPy**: For numerical operations.  
- **Matplotlib**: For visualizations.  
- **TensorFlow/Keras**: For deep learning model implementation.  

You can install all dependencies using the `requirements.txt` file.

---
## Input Analysis
The .wav file which were used in this project are 
1. **Saregama** - Basic chords in music form the foundation of harmony and are built from three or more notes played together. The most common types include major chords, which sound bright and happy (e.g., C major: C-E-G), and minor chords, which have a sadder, more melancholic tone (e.g., A minor: A-C-E). Other essential chords include diminished (tense and unstable), augmented (mysterious and unresolved), and seventh chords, which add depth and complexity to a progression. Mastering these basic chords is key to playing most songs and understanding musical structure.

2. **Blinding Lights** - The intro of Blinding Lights by The Weeknd features a nostalgic, pulsating synthwave melody inspired by 1980s electronic music. It opens with a driving, arpeggiated synth pattern that instantly sets an energetic and retro-futuristic mood. The bright, shimmering synths, combined with a steady four-on-the-floor drumbeat, create a sense of urgency and excitement. The reverb-heavy atmosphere and warm analog-style synth tones give it a cinematic feel, reminiscent of classic ’80s synth-pop soundtracks. This iconic intro builds anticipation before The Weeknd’s vocals enter, making it one of the most recognizable and exhilarating openings in modern pop music.
---

## Code Workflow  

1. **Audio Loading and Preprocessing**  
   - Load the custom audio file.  
   - Extract features using `librosa` (e.g., MFCC, chroma, spectral contrast).  

2. **Model Prediction**  
   - The pre-trained deep learning model processes the audio features and predicts the corresponding chord symbols.  

3. **Visualization**  
   - Generate the waveform and spectrogram of the audio file.  
   - Display predicted chords in the console.
  
---

## List of Chords and Beats

| Chord/ Note Names | Beat Duration | Symbol |
|-------------------|--------------|--------|
| Whole Note       | 4 Beats      | O      |
| Half Note        | 2 Beats      | D      |
| Quarter Note     | 1 Beat       | Q      |
| Eighth Note      | ½ Beats      | E      |
| Sixteenth Note   | ¼ Beats      | S      |
| Whole Rest       | Hold 4 Beats | (Hanging Block) |
| Half Rest        | Hold 2 Beats | (Sitting Block) |
| Quarter Rest     | Hold 1 Beat  | Z      |
| Eighth Rest      | Hold ½ Beats | r      |
| Sharp           | Raises pitch by half a step | # |
| Flat            | Lowers pitch by half a step | b |
| Treble Clef     | G clef, Treble Notes | G |
| Bass Clef       | F clef, Bass Notes | F |
| Staff           | 5 Lines, 4 Spaces | 5L |
| Bar Line        | Divides Measure | - |
| Dotted Note     | Adds Half the Beat Value | Q |



---

## Project Structure  
```
audio-analysis-chord-recognition/  
│  
├── data/                     # Directory for storing audio files  
├── models/                   # Pre-trained model files  
├── VoicePitchDetection.ipynb          # Main script for running the project  
├── requirements.txt           # Python dependencies  
└── README.md                  # Project documentation  
```

---

## Sample Results  

- **Waveform and Spectrogram Visualization**  
  ![Waveform](https://example.com/waveform_image.png)  
  ![Spectrogram](https://example.com/spectrogram_image.png)  

- **Predicted Chords:**  
  `C Major → G Major → A Minor → F Major`

---

## Future Enhancements  
- Add support for more audio formats (MP3, FLAC).  
- Improve chord prediction accuracy with advanced neural networks.  
- Add a web-based interface for easier interaction.

---
