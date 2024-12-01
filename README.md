# ACAI-YOLOv5

## Abstract

This project addresses the challenge of identifying military aircraft from aerial images using computer vision (CV) techniques. For this project, we created a dataset of labeled aircraft using RoboFlow to demonstrate the capabilities of our models to learn and recognize different vehicles. We then applied data augmentation techniques to increase the effectiveness of our dataset and models.

The study explores the performance of three different CV models—YOLOv5, YOLOv8, and a custom deep learning implementation (ConvNet) built using PyTorch. YOLOv5 and YOLOv8, designed and documented by Ultralytics, were implemented as baseline models for comparison. Our custom model was designed to address shortcomings observed in the baseline models, focusing on balancing computational efficiency and detection accuracy. By evaluating these models, we identified performance trade-offs and gained valuable insights into optimizing CV models for accurate aircraft detection in realistic datasets.

---

## GitHub Repository Structure

This repository is a submodule of the Aircraft Classification from Arial Imagery repo linked in the about section:

```mermaid
graph TD
    A[Aircraft-Classification]

    A --> B[YOLOv5]

    B --> B1[train.py]
    B --> B2[dataset/]
    B --> B3[README.md]
```

---

## Evaluation Metrics

Evaluation metrics can be found in the "runs/train/exp." folder after the code has been run. This will include the following:

- **Confusion Matricies**
- **Precision-Confidence Curves**
- **Recall-Confidence Curves**
- **Precision-Recall Curves**
- **F1-Confidence Curves**

---

## Getting Started

### **Prerequisites**

- Python 3.8 or higher
- Required Python packages: Listed in `requirements.txt` within each model submodule
- CUDA-enabled GPU (recommended)

### **Commands**

Run the following command to isntall required libraries:

```bash
    pip install -r requirements.txt
```

Run the following command to get the test results from the report:

```bash
    python train.py --img 640 --batch 16 --epochs 30 --data data.yaml --weights yolov5s.pt
```

---

## Authors

**Alexander Green** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Master of Science in Computer Engineering (MSCpE)<br>
Dept. of Electrical and Computer Engineering, University of Central Florida<br>
[GitHub Home](https://github.com/alexneilgreen)

**Joshua Glaspey** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Master of Science in Computer Engineering (MSCpE)<br>
Dept. of Electrical and Computer Engineering, University of Central Florida<br>
[GitHub Home](https://github.com/jkglaspey)
