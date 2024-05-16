# Drowsiness-Detection-System
Sure, here's a README.md template for your drowsiness detection script:

This Python script detects drowsiness in real-time by analyzing the eye aspect ratio of a person captured through a webcam feed. When the eye aspect ratio falls below a certain threshold for a specified number of consecutive frames, an alarm is triggered to alert the person.

## Requirements

- Python 3.x
- OpenCV
- dlib
- imutils
- numpy
- pygame

You can install the required packages using pip:

```
pip install opencv-python dlib imutils numpy pygame
```

## Usage

1. Clone the repository or download the script.
2. Make sure you have the required libraries installed.
3. IMPORTANT

  Download `shape_predictor_68_face_landmarks.dat.bz2` from [Shape Predictor 68 features](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) 
  Extract the file in the project folder using 
  ``bzip2 -dk shape_predictor_68_face_landmarks.dat.bz2``

4. Run the script using Python:

```
python drowsiness_detection.py
```

4. A webcam window will open displaying the live feed with face detection and eye aspect ratio analysis.
5. If the script detects drowsiness (i.e., when the eye aspect ratio falls below the threshold for a certain number of frames), an alarm will be triggered.

## Configuration

- You can adjust the thresholds and parameters in the script according to your requirements:
  - `EYE_ASPECT_RATIO_THRESHOLD`: Minimum eye aspect ratio below which an alarm is triggered.
  - `EYE_ASPECT_RATIO_CONSEC_FRAMES`: Minimum consecutive frames for which the eye aspect ratio is below the threshold for the alarm to be triggered.

## Credits

- The script utilizes the dlib library for facial landmark detection and OpenCV for face detection.
- The concept of drowsiness detection based on eye aspect ratio is inspired by research in the field of driver fatigue detection.

## License

This project is licensed under the [MIT License](LICENSE).

---
