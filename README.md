# 🚗 Automatic License Plate Recognition (ALPR) System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![YOLO](https://img.shields.io/badge/YOLO-Object%20Detection-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 🎯 Project Overview
This project is a high-performance **License Plate Recognition System** developed to detect and read vehicle license plates from real-time video feeds and static images. 

Leveraging the power of **YOLO (You Only Look Once)** architecture for object detection and **Optical Character Recognition (OCR)** techniques, the system achieves high accuracy even in challenging lighting conditions and angles.

I developed this project to address the need for automated vehicle tracking systems, focusing on optimizing the detection pipeline for speed and accuracy.

## 🛠️ Technical Architecture
The project follows a modular pipeline approach:
1.  **Input Processing:** Capturing video frames or images via OpenCV.
2.  **Object Detection:** Using a custom-trained **YOLO model** (`best.pt`) to localize the license plate region within the frame.
3.  **Image Preprocessing:** Applying grayscale conversion, thresholding, and contour detection to prepare the plate image for OCR.
4.  **Text Recognition (OCR):** Extracting alphanumeric characters from the processed plate image.
5.  **GUI & Logging:** Displaying results on a user-friendly interface (`License_Plate_Recognition_GUI.py`) and logging detected plates to `plates.txt`.

## 📂 Project Structure
```text
├── best.pt                          # Custom trained YOLO model weights
├── License_Plate_Recognition_GUI.py # Main application with Graphical User Interface
├── plates.txt                       # Log file for detected license plates
├── Sample_Data/                     # Sample images/videos for testing
├── Model_Accuracy_Table.jpg         # Confusion matrix and performance metrics
└── README.md                        # Project documentation
```
## 🚀 Key Features
*Real-time Detection: Process video streams with low latency.

*Custom Trained Model: The model was trained specifically on Turkish license plate datasets to handle local fonts and formats.

*GUI Integration: A dedicated interface to upload videos/images and view results instantly.

*Data Logging: Automatically saves detected plate numbers for database integration.

## 📊 Model Performance
The custom YOLO model demonstrates robust performance in detecting plates even with partial occlusion.

(See Model_Accuracy_Table.jpg for detailed metrics)

## 💻 Installation & Usage
**Clone the repository**

```Bash

git clone https://github.com/Vooguz/License-Plate-Recognition-YOLO.git
cd License-Plate-Recognition-YOLO
Install Dependencies
```
```Bash

pip install ultralytics opencv-python easyocr
Run the Application
```
```Bash

python License_Plate_Recognition_GUI.py
```

## 👨‍💻 Author
Oğuz Eren
Computer Engineering Student @Uludağ University

Contact: oueren81@gmail.com
