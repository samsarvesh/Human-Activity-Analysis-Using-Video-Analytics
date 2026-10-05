# Human Activity Analysis Using Video Analytics

## 📌 Project Overview

This project analyzes human activity in a 10-second video using multiple computer vision and deep learning techniques. The system extracts video frames and applies different video analytics approaches to understand human movement, visual features, temporal patterns, and frame-to-frame relationships.

The project generates **eight different visualizations** and combines them into a single composite output.

## 🎯 Aim

To analyze human activity in a 10-second video using different video analytics techniques and visualize the extracted spatial, motion, and temporal features.

## 🔍 Techniques Used

1. **Person Detection** – YOLOv8 is used to detect humans in the video.
2. **Optical Flow** – Farneback Optical Flow is used to visualize movement between consecutive frames.
3. **Motion History** – Motion History representation is generated to show accumulated movement.
4. **CNN Features** – ResNet18 is used to extract visual features from individual frames.
5. **CNN-LSTM** – CNN features are passed through an LSTM to represent temporal information.
6. **3D CNN** – R3D-18 is used to extract spatiotemporal features from the video.
7. **Transformer-Based Analysis** – Cosine similarity between frame features is used to visualize relationships between frames.
8. **Composite Visualization** – All eight outputs are displayed in a single 2×4 visualization.

## 🛠️ Technologies Used

* Python
* Google Colab
* OpenCV
* NumPy
* Matplotlib
* PyTorch
* Torchvision
* Ultralytics YOLOv8
* Scikit-learn

## 📂 Project Workflow

```text
Input Video
     ↓
Frame Extraction
     ↓
10-Second Video Selection
     ↓
┌─────────────────────────────┐
│     Video Analytics         │
├─────────────────────────────┤
│ Person Detection            │
│ Optical Flow                │
│ Motion History              │
│ CNN Feature Extraction      │
│ CNN-LSTM Temporal Features  │
│ 3D CNN Representation       │
│ Transformer Similarity       │
└─────────────────────────────┘
     ↓
Feature Visualization
     ↓
8-Panel Composite Output
```

## 📊 Expected Output

The final output contains:

| No. | Visualization                      |
| --- | ---------------------------------- |
| 1   | Original Video                     |
| 2   | Person Detection                   |
| 3   | Optical Flow                       |
| 4   | Motion History                     |
| 5   | CNN Features                       |
| 6   | CNN-LSTM Feature Sequence          |
| 7   | 3D CNN Video Representation        |
| 8   | Transformer-Based Frame Similarity |

All eight visualizations are combined into a single composite image.

## 🚀 How to Run

### 1. Open Google Colab

Upload the provided `.ipynb` notebook to Google Colab.

### 2. Upload the Video

Run the video upload cell and select a video containing human activity.

### 3. Install Dependencies

The notebook automatically installs the required YOLO package.

```bash
pip install ultralytics
```

### 4. Run the Notebook

Execute the cells sequentially.

The notebook will:

* Read the video
* Extract the first 10 seconds
* Select representative frames
* Detect people
* Calculate optical flow
* Generate motion history
* Extract CNN features
* Generate CNN-LSTM temporal features
* Generate 3D CNN video features
* Calculate frame similarity
* Generate the final composite visualization

## 📁 Output

The final visualization is saved as:

```text
human_activity_analysis.png
```

## 🧠 Key Learning Outcomes

This project demonstrates how different computer vision and deep learning techniques can be applied to video data:

* Object/person detection
* Motion estimation
* Temporal motion representation
* Image feature extraction
* Sequence modeling
* Spatiotemporal feature extraction
* Frame relationship analysis
* Visualization of video features

## ⚠️ Note

The CNN-LSTM, 3D CNN, and Transformer sections in this project demonstrate **feature and representation extraction**. They do not perform actual human activity classification.

Actual activity classification such as **walking, running, jumping, sitting, etc.** requires a trained activity-recognition model and an appropriate labeled dataset.

## 👨‍💻 Project

**Project Title:** Human Activity Analysis Using Video Analytics

**Platform:** Google Colab

**Language:** Python

**Domain:** Computer Vision / Video Analytics / Deep Learning
