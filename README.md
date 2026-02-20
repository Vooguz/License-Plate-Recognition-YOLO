# 🚗 Automatic License Plate Recognition (ALPR) System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLO-v8-orange?style=for-the-badge&logo=ultralytics&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?style=for-the-badge&logo=opencv&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-Latest-red?style=for-the-badge&logo=pytorch&logoColor=white)

## 🎯 Project Overview
This project is a high-performance **License Plate Recognition System** developed to detect and read vehicle license plates from real-time video feeds and static images. 

Leveraging the power of **YOLO (You Only Look Once)** architecture for object detection and **Optical Character Recognition (OCR)** techniques, the system achieves high accuracy even in challenging lighting conditions and angles. It focuses on optimizing the detection pipeline for both speed and reliability.

## 🚀 Application Demo
The following screenshot demonstrates the system's ability to detect the license plate area and successfully convert the visual information into digital text (OCR) through a user-friendly interface.

![Application Screenshot](assets/app_demo.png)

## 🛠️ Technical Architecture
The project follows a modular pipeline approach:
1. **Input Processing:** Capturing video frames or images via OpenCV.
2. **Object Detection:** Using a custom-trained **YOLO model** (`best.pt`) to localize the license plate region.
3. **Image Preprocessing:** Grayscale conversion and thresholding to optimize for character recognition.
4. **Text Recognition (OCR):** Extracting alphanumeric characters from the processed plate image.
5. **GUI & Logging:** Displaying results on a Graphical User Interface and logging detections to `plates.txt`.

## 📊 Model Performance
The custom YOLO model demonstrates robust performance. Below are the training metrics and confusion matrix showcasing the model's accuracy:

![Model Accuracy](assets/Model_Accuracy_Table.jpg)

## 📂 Project Structure
```text
├── assets/                          # Images for documentation (Demo & Graphs)
├── best.pt                          # Custom trained YOLO model weights
├── License_Plate_Recognition_GUI.py # Main application GUI
├── plates.txt                       # Log file for detected license plates
├── requirements.txt                 # Project dependencies
├── Sample_Data/                     # Sample images/videos for testing
└── README.md                        # Project documentation
```

💻 Installation & Usage
1. Clone the Repository
```Bash

git clone [https://github.com/Vooguz/License-Plate-Recognition-YOLO.git](https://github.com/Vooguz/License-Plate-Recognition-YOLO.git)
cd License-Plate-Recognition-YOLO
2. Install Dependencies
```

```Bash

pip install -r requirements.txt
3. Run the Application
```

```Bash

python License_Plate_Recognition_GUI.py
```

✨ Key Features
Real-time Detection: High-speed processing for video streams.

Custom Trained Model: Specifically optimized for local license plate formats and fonts.

OCR Integration: Converts visual plates into searchable text data.

Logging: Automatically saves detected numbers for database integration.

👨‍💻 Author: Oğuz Eren

Computer Engineering Student @ Uludağ University

Contact: oueren81@gmail.com

