

# Face Recognition from Scratch with KNN

**Repository:** [xgagandeep/Face-Recognition-from-Scratch-with-knn](https://github.com/xgagandeep/Face-Recognition-from-Scratch-with-knn)  
**Date:** 2020  
**Language:** Python  
**Libraries:** OpenCV, NumPy

## Description

This project implements a face recognition system using the k-Nearest Neighbors (KNN) algorithm from scratch. The notebook demonstrates how to capture real-time video feed, detect faces, and recognize them based on previously stored face data.

## Features

- **Real-Time Face Detection:** Uses OpenCV's Haar Cascade Classifier to detect faces in a video feed.
- **Face Recognition:** Implements KNN to recognize faces by comparing them with a dataset of known faces.
- **Real-Time Display:** Displays the video feed with bounding boxes and recognized names overlaid on detected faces.

## Files

- **`face recognition knn.ipynb`:** Jupyter Notebook containing the implementation of the face recognition system using KNN.

## Installation

To run this project, you need Python and the required libraries installed. Follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/xgagandeep/Face-Recognition-from-Scratch-with-knn.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd Face-Recognition-from-Scratch-with-knn
   ```

3. **Install the required libraries:**

   ```bash
   pip install numpy opencv-python
   ```

4. **Download the Haar Cascade XML file:**

   The Haar Cascade XML file (`haarcascade_frontalface_alt.xml`) is used for face detection. You can download it from the [OpenCV GitHub repository](https://github.com/opencv/opencv/tree/master/data/haarcascades) and place it in the appropriate directory.

5. **Prepare the face data:**

   Ensure you have a directory (`data`) with face data files saved in `.npy` format. These files should contain face images in numpy array format, where each file corresponds to a different person.

6. **Run the Jupyter Notebook:**

   ```bash
   jupyter notebook face\ recognition\ knn.ipynb
   ```

## Usage

1. **Face Data Preparation:**
   - Load existing face data from `.npy` files.
   - Combine face data and labels into a single dataset for training.

2. **Real-Time Face Recognition:**
   - Capture video feed from the camera.
   - Detect faces using Haar Cascade.
   - Extract face sections, resize them, and flatten for KNN classification.
   - Display the recognized face name on the video feed.

3. **Exit the Application:**
   - Press 'q' to quit the video feed and close the application.

## Functions

- **`dist(X1, X2)`**: Computes the Euclidean distance between two vectors.
- **`knn(X, Y, Query, k=5)`**: Applies KNN to classify a query face based on a dataset of known faces.
- **`cv2.VideoCapture("0")`**: Captures video feed from the default camera.
- **`cv2.CascadeClassifier()`**: Loads the Haar Cascade classifier for face detection.
- **`cv2.imshow()`**: Displays the video feed with detected and recognized faces.

## Example

The notebook captures real-time video, detects faces, and recognizes them based on pre-trained face data. Make sure to have your `data` directory set up with face images and update the paths accordingly.

## Contribution

Feel free to contribute to this project by submitting issues or pull requests. For any questions or feedback, please open an issue on the GitHub repository.
