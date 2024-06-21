# Face Detection and Recognition System using AI

This project implements a real-time face recognition and detection system using dlib's face detection and face recognition capabilities along with OpenCV for image processing. It allows you to recognize faces in a live video stream from your webcam or from a video file.

## Features

- Detects faces in real-time using dlib's pre-trained face detector.
- Recognizes faces by comparing face descriptors using a pre-trained face recognition model.
- Allows adding new faces to the system dynamically.
- Displays recognized faces with their names in the video stream.
- Simple interface for adding new faces when an unknown face is detected.

## Requirements

1. Python 3.x
2. OpenCV (`pip install opencv-python`)
3. dlib (`pip install dlib`)
4. NumPy (`pip install numpy`)
5. requests (`pip install requests`) - for downloading the pre-trained models
6. bz2 (usually included in Python standard library)

## Setup

### 1. Clone the repository:
   
   ```bash
   git clone https://github.com/Reyajosephine/CODSOFT.git
   cd FACE-DETECTION
   ```

### 2. Install Dependencies:
- Navigate to the project directory and install the required Python dependencies using pip:

```bash
cd Face_Recognition
pip install -r requirements.txt
```

### 3. Download Models:
- The script automatically downloads the required face detection and recognition models. However, if you encounter any issues, manually download the following models:
1. `shape_predictor_68_face_landmarks.dat`
2. `dlib_face_recognition_resnet_model_v1.dat`

### 3. Prepare Known Faces:
- Add images of known faces to the known_faces directory.
- Ensure the images are named appropriately and contain only the face of the person to be recognized.

## Usage
- The system will start capturing frames from the selected video source (webcam or file).
- Detected faces will be highlighted with a bounding box and labeled with their names if recognized.
- If an unknown face is detected, a separate window will prompt you to add a name for that face.
- Press '**a**' to add the face with a new name.
- Press '**c**' to continue without adding the face.
- Added faces are stored persistently in `known_faces.json`.
  
## Contributions
Contributions are welcome! If you have any improvements or feature suggestions, feel free to fork the repository and submit a pull request. Please ensure to follow the existing code style and add relevant tests if applicable.

## License
This project is licensed under the MIT License - see the LICENSE file for details.


   
