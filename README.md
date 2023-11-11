# Emotion-Based Music Player

## Introduction

The Emotion-Based Music Player is a Python project that utilizes facial recognition to detect emotions and play music accordingly. It combines computer vision techniques, emotion recognition, and a simple graphical user interface created with Eel to provide an interactive music experience.

## Features

1. **Emotion Detection:** The system can recognize emotions such as angry, happy, sad, and neutral based on facial expressions.

2. **Music Player:** It features a built-in music player that plays songs corresponding to the detected emotion.

3. **Queue Mode:** Users can create a queue of songs to be played consecutively.

4. **Emotion Mode:** The system automatically selects songs based on the user's detected emotion.

5. **Random Mode:** Play random songs from the playlist.

## Project Structure

- **WD Folder:** Contains web-related files for the Eel GUI.
  - `main.html`: The main HTML file for the GUI.
  - `header.css`, `background.css`, `player.css`: CSS files for styling.
  - `code.js`: JavaScript file for handling GUI interactions.
  - `eel.js`: Eel library file.

- **Images Folder:** Contains images used in the GUI.

- **Capture.py:** The main script for capturing facial expressions and updating the dataset.

- **Update_Model.py:** Script for updating the emotion detection model.

- **Light.py:** Module for controlling the lighting conditions during face capture.

- **Haarcascade_frontalface_default.xml:** Haarcascade XML file for face detection.

## System Requirements

- Python 3.x
- OpenCV
- Eel
- Other dependencies (see `requirements.txt`)

## Installation (IMPORTANT)

 Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage
### Note: Make sure you have a camera connected to your computer or ensure it is turned on before running the code.

1. Navigate to the project directory:

   ```bash
   cd emotion-based-music-player
   ```

2. Run the main script:

   ```bash
   python capture.py
   ```

3. The GUI will open, and the system will start capturing facial expressions.

4. Follow on-screen instructions to capture emotions for model training.

5. Enjoy the music based on your detected emotion!

## Options

- **Hard Update (Optional):**
If you have a predefined dataset, use hard_update.py to perform a hard update of the emotion recognition model.

  ```bash
  python hard_update.py
  ```

## Troubleshooting

- **AttributeError: module 'cv2' has no attribute 'face':**
  If you encounter this error, ensure that the required OpenCV modules are installed:

  ```bash
  pip install opencv-python opencv-contrib-python
  ```
