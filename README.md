# DL_IA2_16014224811_16014224812
Deep learning IA2

#  Solar Panel Defect Classification using Deep Learning

##  Overview

This project focuses on detecting and classifying defects on solar panels using deep learning. Environmental factors like dust, snow, bird droppings, and damages reduce solar panel efficiency. This model automates inspection using image classification.

---

##  Objective

To build a multi-class image classification model that identifies:

* Clean
* Dusty
* Bird-drop
* Electrical Damage
* Physical Damage
* Snow Covered

---

##  Model

* **Architecture:** EfficientNet-B3 (Transfer Learning)
* **Framework:** PyTorch
* **Fine-tuning:** Last 2 blocks
* **Custom Head:** Fully Connected layers with Dropout & BatchNorm

---

##  Techniques Used

* Data Augmentation (flip, rotation, color jitter, blur, erasing)
* Weighted Sampling (class imbalance handling)
* Mixup Augmentation
* Label Smoothing
* Differential Learning Rates
* Warmup + Cosine LR Scheduler
* Test-Time Augmentation (TTA)

---

## Results

* Validation Accuracy: **86.9%**
* Test Accuracy: **78.7%**
* TTA Accuracy: **87.23%**
* Macro F1 Score: **~0.80**

---

##  Dataset

[Kaggle Solar Panel Dataset](https://www.kaggle.com/datasets/pythonafroz/solar-panel-images)

---

##  How to Run

```bash
pip install -r requirements.txt
```

Run notebook:

```bash
jupyter notebook
```



## Authors

* Rishi Mane
* Nimit Mehta
