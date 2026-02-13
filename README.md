# NumberPlate-detection

🔎 Number Plate Detection using YOLOv8
📌 Project Overview
This project implements automatic number plate detection using a custom-trained YOLOv8 model. The system can detect and localize vehicle license plates in real-time from images or video streams. It is designed for applications such as:

Intelligent traffic monitoring

Automated toll collection

Parking management systems

Law enforcement and surveillance

✨ Features
Custom Dataset: Annotated vehicle number plates for YOLOv8 training.

High Accuracy: Achieves strong mAP scores on diverse datasets.

Real-Time Performance: Optimized for video streams and CCTV footage.

Scalable: Works across different regions, plate formats, and lighting conditions.

🛠️ Tech Stack
Framework: Ultralytics YOLOv8

Language: Python

Libraries: OpenCV, PyTorch, NumPy

Environment

🚀 Getting Started
1. Clone the repository

   
bash
git clone https://github.com/your-username/numberplate-detection-yolov8.git


cd numberplate-detection-yolov8

2. Install dependencies
bash
pip install -r requirements.txt

3. Train the model
bash
yolo task=detect mode=train model=yolov8n.pt data=data.yaml epochs=50 imgsz=640

4. Run inference
bash
yolo task=detect mode=predict model=models/best.pt source=video.mp4

📊 Results
mAP@50 > 90% on custom dataset

Real-time detection at ~30 FPS on GPU

Robust detection across multiple plate formats

🔮 Future Work
OCR integration for automatic plate recognition (ANPR).

Deployment on edge devices (Jetson Nano, Raspberry Pi).

Multi-country plate format support.
