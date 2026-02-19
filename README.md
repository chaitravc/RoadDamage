
# Road Damage Detection System

Road Damage Detection is an AI-powered web application that detects and classifies road surface damages such as potholes and cracks from images, videos, and real-time camera feeds using deep learning.

The system uses a YOLOv8-based object detection model and provides an interactive Streamlit multi-page web interface for easy testing and visualization of results.

---

## Project Overview

Poor road conditions significantly impact transportation safety and maintenance costs. Manual inspection methods are slow, expensive, and error-prone.

This project automates road damage detection by:
- Identifying damaged road areas
- Highlighting damages with bounding boxes
- Supporting real-time, image, and video-based detection
- Providing an easy-to-use web interface

---

## Features

- Real-time road damage detection using webcam
- Image-based detection through file upload
- Video-based detection for recorded footage
- Fast and accurate detection using YOLOv8
- Streamlit-powered multi-page web application
- Modular and scalable project structure

---

## How It Works

### Client Side (Streamlit UI)
- User selects detection mode from sidebar
- Uploads image or video, or enables webcam
- Displays detection results with bounding boxes
- Shows confidence scores for detected damages

### Model and Backend Logic
- YOLOv8 model loads from pre-trained `.pt` file
- Input frames are processed using OpenCV
- Detected objects are drawn and returned to UI
- Optimized for CPU execution

---

## Tech Stack

- Frontend: Streamlit
- Deep Learning Model: YOLOv8 (Ultralytics)
- Programming Language: Python
- Computer Vision: OpenCV
- Model Framework: PyTorch
- Runtime Environment: Local (CPU)

---

## Project Structure

```

RoadDamageDetection/
│
├── .streamlit/
├── models/
│   └── YOLOv8_Small_RDD.pt
│
├── pages/
│   ├── 1_Realtime Detection.py
│   ├── 2_Image Detection.py
│   └── 3_Video Detection.py
│
├── resource/
├── sample_utils/
│   ├── download.py
│   └── get_STUNServer.py
│
├── training/
├── Home.py
├── requirements.txt
├── packages.txt
├── README.md
└── .gitignore

````

---

## Setup Instructions

### Clone Repository
```bash
git clone https://github.com/oracl4/RoadDamageDetection.git
cd RoadDamageDetection
````

---

### Create Virtual Environment (Python 3.10 recommended)

Do not uninstall existing Python versions.

```bash
py -3.10 -m venv venv
```

Activate the virtual environment:

Windows:

```bash
venv\Scripts\activate
```

---

### Install Dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

---

### Run the Application

```bash
streamlit run Home.py
```

---

## How to Use

1. Open the browser link shown in the terminal (usually [http://localhost:8501](http://localhost:8501))
2. Use the sidebar to select:

   * Real-Time Detection
   * Image Detection
   * Video Detection
3. Upload files or enable webcam
4. View detected road damages with bounding boxes

---

## Dependencies

Major dependencies used in this project:

* streamlit
* torch
* ultralytics
* opencv-python-headless
* numpy
* Pillow
* requests
* streamlit-webrtc

Refer to `requirements.txt` for the complete list.

---

## Output

* Detection of road damages with bounding boxes
* Confidence scores for detected damages
* Support for real-time, image, and video inputs

---

## Future Enhancements

* Damage severity classification
* GPS-based road damage mapping
* Cloud-based deployment
* Mobile-friendly interface
* Larger and more diverse datasets

---

## Conclusion

This project demonstrates an end-to-end AI-powered road damage detection system using deep learning and an interactive web interface.

It can be used for:

* Smart city infrastructure monitoring
* Road maintenance planning
* Automated inspection systems

Road Damage Detection provides an efficient and scalable solution for identifying road surface damages.

```

---


Just tell me what you need next.
```
