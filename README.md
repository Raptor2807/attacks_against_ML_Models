# attacks_against_ML_Models
# Semester Project
## Goal 
    Implement membership inference attacks against the given pre-trained target models.   
# 🕵️‍♂️ Membership Inference Attacks on Pre-Trained Neural Networks

This project implements Membership Inference Attacks (MIAs) on pre-trained neural networks using the PyTorch framework. It evaluates privacy leakage vulnerabilities in ML models trained on CIFAR10 and Tiny ImageNet datasets using ResNet34 and MobileNetV2 architectures.

## 📌 Goal

To assess whether a given data point was part of a model's training set (member) or not (non-member), thereby evaluating potential privacy risks of deployed machine learning models.

---

## 🛠 Setup

- Python 3.8+
- PyTorch
- NumPy
- Pickle
- TorchVision

Clone the repo and set up the environment:

bash
git clone https://github.com/yourusername/membership-inference-attack.git
cd membership-inference-attack
pip install -r requirements.txt

## Supported Datasets
CIFAR10

Tiny ImageNet

## Data Files per Task
shadow.p – Used to train the shadow and attack models.

eval.p – For evaluating attack model performance.

test.p – Final test file for prediction and submission.

Each .p file is a pickled list containing:

shadow.p, test.p: [image, label]

eval.p: [image, label, membership] (1=member, 0=non-member)

## Target Models
ResNet34

MobileNetV2
