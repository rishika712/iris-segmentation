# 👁️ Iris Segmentation Using MediaPipe and Python

This project demonstrates real-time **iris segmentation and tracking** using [MediaPipe's Face Mesh](https://google.github.io/mediapipe/solutions/face_mesh.html) in Python. It utilizes facial landmarks to accurately detect and segment the iris region from live video input.

## 📌 Objective

- Leverage MediaPipe's Face Mesh to detect facial landmarks.
- Extract and segment the iris region using specific landmark indices.
- Visualize the segmented iris in real-time using OpenCV.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:**
  - [MediaPipe](https://pypi.org/project/mediapipe/)
  - [OpenCV](https://pypi.org/project/opencv-python/)
  - NumPy

## 📁 Project Structure

iris-Segmentation-mediapipe-python-master/
├── main.py # Main script for real-time iris segmentation
└── segmentation_mask.py # Module for creating segmentation masks


## 🚀 How to Run the Project

1. **Clone the Repository**

git clone https://github.com/rishika712/iris-segmentation.git
cd iris-segmentation/iris-Segmentation-mediapipe-python-master

2. **Set Up a Virtual Environment (Optional but Recommended)**

**For Linux/macOS:**

python3 -m venv venv
source venv/bin/activate

**For Windows:**

python -m venv venv
venv\Scripts\activate

3. **Install Dependencies**

pip install -r requirements.txt

4. **Run the Application**

python main.py
This will activate your webcam and start the real-time iris segmentation.

## 🎯 How It Works
Face Mesh Detection: Utilizes MediaPipe's Face Mesh solution to detect 468 facial landmarks.

Iris Landmark Extraction: Specific landmark indices correspond to the iris region:

Left Iris: 474, 475, 476, 477

Right Iris: 469, 470, 471, 472

Segmentation Mask: The segmentation_mask.py module processes these landmarks to create a mask highlighting the iris region.

Visualization: OpenCV is used to display the original frame with the segmented iris overlay.

## 📄 License
This project is licensed under the MIT License.
