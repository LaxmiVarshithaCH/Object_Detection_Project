# 🧠 Object Detection Project

This project focuses on building a custom object detection model using the YOLOv5 architecture. The model is trained to detect specific objects from images and videos and can be used for applications like real-time detection, automation, and surveillance.

---

## 📌 Table of Contents

- [🔍 Overview](#-overview)
- [✅ Features](#-features)
- [⚙️ Installation](#️-installation)
- [🚀 How to Use](#-how-to-use)
- [📂 Dataset Structure](#-dataset-structure)
- [🏋️‍♂️ Training Details](#️-training-details)
- [📊 Results](#-results)
- [🖼️ Example Outputs](#-example-outputs)
- [🙋‍♀️ Contributors](#-contributors)
- [📄 License](#-license)
- [📬 Feedback](#-feedback)

---

## 🔍 Overview

This project demonstrates:

- Dataset preparation for object detection
- Model training using YOLOv5
- Result analysis through loss/mAP curves
- Detection on new unseen images

The notebook `object_detector.ipynb` contains the complete pipeline.

---

## ✅ Features

- 📦 Custom object detection
- 📈 Real-time training visualization
- 🖼️ Supports inference on new images
- 🔧 Easy to extend and fine-tune
- 📁 Exports results in image and CSV format

---

## ⚙️ Installation

### 1. Clone this Repository


git clone https://github.com/LaxmiVarshithaCH/Object_Detection_Project.git
cd Object_Detection_Project


### 2. Install YOLOv5 and Dependencies

git clone https://github.com/ultralytics/yolov5
cd yolov5
pip install -r requirements.txt
✅ Ensure Python 3.8+ and PyTorch are installed on your system.

## 🚀 How to Use

### 1. Open the Notebook
Launch Jupyter Notebook or VS Code and open object_detector.ipynb.

### 2. Train the Model
Define the dataset path and number of classes

Start training using YOLOv5 commands in the notebook

### 3. Run Inference
Upload a new image

Run the detection cell

Get bounding boxes and class labels on the image

## 📂 Dataset Structure
<pre> dataset/ ├── images/ │ ├── train/ │ └── val/ ├── labels/ │ ├── train/ │ └── val/ </pre>

Each label file should follow YOLO format:
<class_id> <x_center> <y_center> <width> <height>


## 🏋️‍♂️ Training Details
| Parameter     | Value                                                  |
| ------------- | ------------------------------------------------------ |
| Model         | YOLOv5s                                                |
| Epochs        | 100 (configurable)                                     |
| Batch size    | 16                                                     |
| Image size    | 640x640                                                |
| Optimizer     | SGD or Adam                                            |
| Loss Function | YOLO Loss (Bounding box + Objectness + Classification) |


## 📊 Results
Training metrics are saved in:

runs/train/exp/results.png — Loss, precision, recall, mAP

runs/train/exp/results.csv — Epoch-wise logs

Example:
| Metric    | Value |
| --------- | ----- |
| mAP\@0.5  | 0.89  |
| Precision | 0.92  |
| Recall    | 0.87  |


## 🖼️ Example Outputs
| Input Image                | Output with Detections       |
| -------------------------- | ---------------------------- |
| ![myimage](https://github.com/user-attachments/assets/d556c770-5f5b-4366-896f-fbf8ca135a4e) | ![download (1)](https://github.com/user-attachments/assets/d536bd72-774e-4f8a-a963-2aabbeb1f8af) |


## 🙋‍♀️ Contributors
CHENNUPALLI LAXMI VARSHITHA
GitHub: @LaxmiVarshithaCH

## 📄 License
This project is licensed under the MIT License.
Feel free to use, modify, and distribute it for personal or commercial use.

## 📬 Feedback
Have suggestions or improvements?
Feel free to open an issue or submit a pull request. Happy coding! 🚀
