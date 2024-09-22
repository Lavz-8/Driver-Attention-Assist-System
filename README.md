# Driver-Attention-Assist-System

## Overview
To avoid the Accidents and drowsiness  of the driver, the alarm which is install in this project will detect and capture the sleepy drivers within 3-5 seconds. This project implements a Driver Attention Assist System using a webcam feed to detect drowsiness in real-time. The system uses dlib to calculate the Eye Aspect Ratio (EAR) and triggers an alarm if the driver appears drowsy for a sustained period.

## Features
- Drowsiness Detection: Monitors the driver’s eyes and detects signs of drowsiness.
- Real-time Processing: Uses webcam feed to provide real-time feedback.
- Alarm System: Plays an alarm sound if drowsiness is detected.
- Face Detection: Uses Haar cascade for initial face detection.

## Installation

1. **Clone this repository to your local machine:**

    ```bash
    git clone https://github.com/Lavz-8/driver-attention-assist-system.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd driver-attention-assist-system
    ```
 
3. **Install the required Python packages:**

    ```bash
    pip install -r requirements.txt
    ```
    
4. **Download the dlib shape predictor model:**

- Download the `shape_predictor_68_face_landmarks.dat` file from dlib's model zoo and extract it into the project directory.

5. **Ensure you have the Haarcascade XML file:**

- Ensure `haarcascade_frontalface_default.xml` is in the haarcascades directory. If not, download it from [OpenCV's GitHub repository](https://github.com/opencv/opencv/tree/master/data/haarcascades).
  
6. **Ensure you have an alarm sound file:**

Place your alarm sound file (e.g.,`alarm.wav`) in the audio directory or update the script with the correct path to your audio file.

## Usage

1. **Run the script:**

    ```bash
    python driver_attention_assist.py
    ```
    
2. **Monitor the output:**

- The webcam feed will start, and the system will monitor the driver’s eyes.
- Rectangles will be drawn around detected faces, and eye contours will be highlighted.
- An alarm will sound if the EAR drops below the threshold for a sustained period, indicating drowsiness.
  
3. **Stop the script:**

-Press `q` to quit the video feed and stop the script.

## Output

### Driver Before Drowsiness
![IMG-20230523-WA0002](https://github.com/Lavz-8/Driver-Attention-Assist-System/assets/171010558/0d34c292-a698-4261-b672-103198545d22)

### Driver After Drowsiness
![IMG-20230523-WA0001](https://github.com/Lavz-8/Driver-Attention-Assist-System/assets/145861363/700b804d-bda0-42d0-b285-b315c1a58626)

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests.

## Credits
This Driver Attention Assist System was created by Your **Lavanya Varadharajan**.
