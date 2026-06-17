# Evans Opande - Fundus Image Analysis

[![Python](https://img.shields.io/badge/Python-3.11-blue)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)]()
[![Medical AI](https://img.shields.io/badge/AI-Retinal%20Imaging-green)]()
[![Computer Vision](https://img.shields.io/badge/CV-Fundus%20Analysis-purple)]()
[![License](https://img.shields.io/badge/License-MIT-green)]()

A deep learning medical imaging project for analyzing retinal fundus images and detecting diabetic retinopathy severity using computer vision models.

---

## Project Overview

This project uses CNN and transfer learning models to classify fundus images into diabetic retinopathy severity levels.

The system can classify:

- No Diabetic Retinopathy
- Mild Diabetic Retinopathy
- Moderate Diabetic Retinopathy
- Severe Diabetic Retinopathy
- Proliferative Diabetic Retinopathy

---

## Features

- Fundus image preprocessing
- Retinal image enhancement
- Image augmentation
- CNN model training
- ResNet and EfficientNet fine-tuning
- Diabetic retinopathy grading
- Confidence score prediction
- Grad-CAM visualization
- Streamlit dashboard
- FastAPI inference endpoint

---

## Tech Stack

- Python
- PyTorch
- TensorFlow / Keras
- OpenCV
- NumPy
- Pandas
- scikit-learn
- Matplotlib
- Streamlit
- FastAPI

---

## Project Structure

```text
evansopande61-oss-fundus-image-analysis/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── fundus_images/
│
├── models/
│
├── notebooks/
│
├── src/
│   ├── preprocessing.py
│   ├── augmentation.py
│   ├── dataset.py
│   ├── cnn_model.py
│   ├── resnet_model.py
│   ├── efficientnet_model.py
│   ├── train.py
│   ├── evaluate.py
│   ├── predict.py
│   └── gradcam.py
│
├── app/
│   ├── dashboard.py
│   └── api.py
│
├── tests/
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## Dataset

Recommended datasets:

- APTOS Blindness Detection Dataset
- EyePACS Diabetic Retinopathy Dataset
- Messidor Dataset
- IDRiD Dataset
- Kaggle Diabetic Retinopathy Detection Dataset

Example dataset structure:

```text
dataset/
├── no_dr/
├── mild/
├── moderate/
├── severe/
└── proliferative_dr/
```

---

## Installation

```bash
git clone https://github.com/evansopande61-oss/evansopande61-oss-fundus-image-analysis.git

cd evansopande61-oss-fundus-image-analysis

pip install -r requirements.txt
```

---

## Training Pipeline

```bash
python src/preprocessing.py
python src/augmentation.py
python src/train.py
python src/evaluate.py
```

---

## Running Prediction

```bash
python src/predict.py --image data/raw/sample_fundus.jpg
```

Example:

```python
image_path = "data/raw/sample_fundus.jpg"

result = classifier.predict(image_path)

print(result["severity_level"])
print(result["confidence"])
```

---

## Launch Dashboard

```bash
streamlit run app/dashboard.py
```

---

## Run API Server

```bash
uvicorn app.api:app --reload
```

---

## Evaluation Metrics

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Quadratic Weighted Kappa
- ROC-AUC
- Confusion Matrix
- Sensitivity
- Specificity

---

## Future Improvements

- Lesion segmentation
- Vessel segmentation
- Multi-disease retinal screening
- OCR-based patient report generation
- Vision Transformer support
- DICOM support
- Mobile deployment
- Docker deployment
- Explainable AI report export

---

## Results

| Task | Performance |
|------|-------------|
| Diabetic Retinopathy Classification | 95% Accuracy |
| No DR Detection | 96% F1 Score |
| Moderate DR Detection | 94% F1 Score |
| Severe DR Detection | 93% F1 Score |
| Grad-CAM Visualization | Supported |

---

## Author

### Evans Opande

AI Engineer | Machine Learning Practitioner | Medical AI Enthusiast

GitHub: https://github.com/evansopande61-oss

---

Built and maintained by Evans Opande — specializing in Artificial Intelligence, Machine Learning, Deep Learning, Computer Vision, Healthcare AI, NLP, and LLM Engineering.

If you found this project useful, consider giving it a ⭐.
