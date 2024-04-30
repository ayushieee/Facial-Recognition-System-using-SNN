# Face Recognition using Siamese Neural Network

This project implements face recognition using a Siamese Neural Network trained on pairs of images. The system captures an input image from a webcam and verifies it against a set of verification images using the trained model.

## Description

The project consists of three main components:

1. **train.py**: This script captures images from a webcam to create datasets for positive, negative, and anchor images. It then preprocesses the data, defines and trains the Siamese Neural Network model using TensorFlow/Keras, and saves the trained model.

2. **layers.py**: This file contains custom layer definitions for the Siamese Neural Network.

3. **faceid.py**: This is the application file which uses the trained model to verify an input image against a set of verification images.

## How to Run

### Requirements

- Python 3.x
- TensorFlow
- OpenCV
- Kivy

### Steps

1. **Clone the Repository**: Clone this repository to your local machine.

   ```bash
   git clone https://github.com/yourusername/facerecognition-siamese.git
   ```

2. **Install Dependencies**: Install the required Python packages.

   ```bash
   pip install tensorflow opencv-python kivy
   ```

3. **Data Collection and Training**: Run the `train.py` script to collect images from your webcam and train the Siamese Neural Network model.

   ```bash
   python train.py
   ```

4. **Run the Application**: Once the model is trained, run the `faceid.py` script to start the face recognition application.

   ```bash
   python faceid.py
   ```

5. **Verification Process**: In the application, click the "Verify" button to capture an input image from your webcam and verify it against the set of verification images.

## Notes

- Make sure to have the webcam connected and properly configured before running the scripts.
- Ensure that the `lfw` dataset is available in the project directory for negative image collection during training.

## Additional Information

For more details about the project implementation, please refer to the source code and comments within each script file.

Enjoy experimenting with face recognition using Siamese Neural Networks! If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.
