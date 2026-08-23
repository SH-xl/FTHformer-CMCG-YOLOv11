# FTHformer-CMCG-YOLOv11

Official implementation of FTHformer-CMCG-YOLOv11 for transmission tower image restoration and defect detection under multiple adverse imaging conditions.

## Overview

UAV-based transmission tower inspection is often affected by adverse imaging conditions, such as haze, rain streaks, snow, raindrops, and motion blur, which degrade image quality and reduce defect detection accuracy.
This repository provides the implementation of **FTHformer-CMCG-YOLOv11**, a sequential image restoration–detection framework that integrates **FTHformer** for degraded image restoration and **CMCG-YOLOv11** for transmission tower defect detection.
The framework is designed to improve defect recognition from degraded UAV images under multiple adverse imaging conditions.

## Framework

The complete processing pipeline is:

```text
Degraded Image
        ↓
FTHformer Image Restoration
        ↓
Restored Image
        ↓
CMCG-YOLOv11 defect detection
        ↓
Defection Results
```

## Environment

The code was developed using:

* Python 3.10
* PyTorch
* CUDA
* Ultralytics
* OpenCV

A CUDA-enabled GPU is recommended for model training.

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/FTHformer-CMCG-YOLOv11.git
cd FTHformer-CMCG-YOLOv11
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Create a virtual environment

Using Conda:

```bash
conda create -n CMCG-YOLO python=3.10 -y
conda activate CMCG-YOLO
```

### 3. Install PyTorch

Install the PyTorch version compatible with your CUDA environment from the official PyTorch website.

For example:

```bash
pip install torch torchvision torchaudio
```

### 4. Install other dependencies

```bash
pip install -r requirements.txt
```

## Results

The proposed framework is evaluated using image restoration and object-detection metrics, including:

* PSNR
* SSIM
* Precision
* Recall
* mAP@0.5
* mAP@0.5:0.95

Detailed results are reported in the corresponding paper.


## Acknowledgements

This project is developed based on:

- PyTorch
- Ultralytics YOLO
- Histoformer

We sincerely thank the developers and contributors of these open-source projects.

## Contact

For questions about this repository, please contact:

```text
Name: YOUR NAME
Email: YOUR EMAIL
```
