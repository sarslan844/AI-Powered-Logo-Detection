# ✈️ AI-Powered Pakistan Air Force Logo Detection using Ultralytics YOLO11

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![YOLO11](https://img.shields.io/badge/Ultralytics-YOLO11-red)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-orange?logo=pytorch)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv)
![License](https://img.shields.io/badge/License-MIT-yellow)

> An AI-powered object detection model for detecting **Pakistan Air Force (PAF) logos** using **Ultralytics YOLO11**.

---

## 📌 Project Overview

This project demonstrates the complete object detection pipeline using **Ultralytics YOLO11**, from manual data collection and annotation to model training, evaluation, and inference.

The primary objective of this project was to gain practical experience in building an end-to-end computer vision solution rather than maximizing benchmark performance.

---

## 🎯 Features

- Manually collected and annotated custom dataset
- End-to-end object detection pipeline
- Transfer Learning using YOLO11
- High detection accuracy
- Training and inference notebooks included
- Ready-to-use trained model (`best.pt`)
- Sample predictions and evaluation results

---

# 📂 Dataset

- **Total Images:** 596
- **Classes:** 1 (Pakistan Air Force Logo)
- **Train Split:** 70%
- **Validation Split:** 20%
- **Test Split:** 10%

The dataset was manually collected and annotated to gain practical experience in dataset preparation and object detection workflows.

Directory structure:

```
dataset/
│
├── train/
├── valid/
├── test/
└── data.yaml
```

---

# 🛠 Tech Stack

- Python
- Ultralytics YOLO11
- PyTorch
- OpenCV
- NumPy
- Google Colab
- Matplotlib

---

# 📊 Validation Results

| Metric | Score |
|---------|-------|
| Precision | **99.83%** |
| Recall | **100.00%** |
| mAP@0.5 | **99.50%** |
| mAP@0.5:0.95 | **88.71%** |

---

# 📈 Evaluation Results

The repository includes:

- Confusion Matrix
- Normalized Confusion Matrix
- Precision Curve
- Recall Curve
- Precision-Recall Curve
- F1 Score Curve

All evaluation plots are available in the **results/** directory.

---

# 🖼 Sample Predictions

Example inference outputs are available inside:

```
predictions/
```

Validation prediction images are available in:

```
results/
```

---

# 📁 Project Structure

```
AI-Powered-PAF-Logo-Detection/
│
├── assets/
├── dataset/
│   ├── train/
│   ├── valid/
│   ├── test/
│   └── data.yaml
│
├── predictions/
├── results/
├── weights/
│   └── best.pt
│
├── train.ipynb
├── predict.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/sarslan844/ai-powered-paf-logo-detection-yolo11.git
```

Go inside the project

```bash
cd ai-powered-paf-logo-detection-yolo11
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🚀 Training

Open the notebook:

```
train.ipynb
```

or train using the Ultralytics CLI:

```bash
yolo detect train \
model=yolo11n.pt \
data=dataset/data.yaml \
epochs=100 \
imgsz=640
```

---

# 🔍 Inference

Run:

```bash
python predict.py
```

Or using the Ultralytics CLI:

```bash
yolo detect predict \
model=weights/best.pt \
source=dataset/sample_images
```

---

# 📈 Learning Outcomes

Through this project, I gained practical experience in:

- Dataset collection
- Image annotation
- Dataset preprocessing
- Transfer Learning
- YOLO11 training
- Model evaluation
- Object detection
- Performance analysis
- Computer Vision workflows

---

# 🚀 Future Improvements

- Increase dataset size
- Detect multiple military logos
- Deploy using Streamlit
- Export model to ONNX
- Real-time webcam detection
- Edge deployment

---

# 👨‍💻 Author

**Arslan Sadiq**

AI & Computer Vision Enthusiast

GitHub: https://github.com/sarslan844

LinkedIn: *(Add your LinkedIn profile URL here)*

---

# 📜 License

This project is licensed under the MIT License.

---

# 🙏 Acknowledgements

- Ultralytics
- PyTorch
- OpenCV
- Google Colabs
