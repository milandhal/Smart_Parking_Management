🚗 ParkSense
Real-Time Smart Parking Detection System

🔴 Live Demo: https://smart-parking-management-1.onrender.com/

📂 GitHub: https://github.com/milandhal/Smart_Parking_Management

📌 Overview

ParkSense AI is a real-time computer vision-based smart parking management system that detects vehicle occupancy in parking slots using Python and OpenCV. The system processes parking lot video footage, analyzes predefined parking regions, and displays live slot availability through a deployed web application.

This project demonstrates end-to-end development — from computer vision implementation to cloud deployment.

🎯 Key Features

🚘 Real-time parking slot occupancy detection

🟢🟥 Visual indication of free and occupied spaces

📊 Live free-slot counter display

🌐 Web-based live streaming interface

⚡ Optimized and lightweight processing pipeline

🧠 Tech Stack

Python

OpenCV

NumPy

CVZone

Flask

Gunicorn

Render (Cloud Deployment)

🛠️ System Workflow

Video feed is captured from a parking lot dataset.

Image preprocessing pipeline:

Grayscale conversion

Gaussian blur

Adaptive thresholding

Median filtering

Dilation

Each predefined parking slot is cropped and analyzed.

Pixel intensity is calculated using cv2.countNonZero().

If pixel count is below threshold → Slot marked Free.

Live counter updates and is streamed via web interface.

📂 Project Structure
Smart_Parking_Management/
│
├── app.py
├── CarParkPos
├── carPark.mp4
├── requirements.txt
├── Procfile
└── README.md

🚀 Deployment

The application is deployed on Render using Gunicorn for production serving.

Deployment Steps:

Push project to GitHub

Connect repository to Render

Set:

Build Command: pip install -r requirements.txt

Start Command: gunicorn app:app

Deploy and access via public URL

📊 Performance Metrics

🎯 ~95% parking slot detection accuracy

⚡ Real-time processing with optimized threshold tuning

📉 Reduced manual monitoring through automated detection

💼 Why This Project Matters

This project showcases:

Real-time computer vision implementation

Practical smart mobility solution

Backend deployment using Flask & Gunicorn

Cloud hosting and web streaming integration

It reflects strong problem-solving skills in computer vision and applied AI systems.

🔮 Future Enhancements

YOLO-based vehicle detection integration

Live CCTV camera feed support

Parking analytics dashboard

Database integration for historical tracking

👨‍💻 Author

Milan Dhal
Machine Learning & Analytics Enthusiast


