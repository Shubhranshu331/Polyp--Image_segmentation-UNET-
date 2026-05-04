# 🧠 Polyp Segmentation using U-Net

## 📌 Overview
This project focuses on **automatic segmentation of polyps in colonoscopy images** using a deep learning model based on the **U-Net architecture**.

Early detection of polyps is crucial for preventing colorectal cancer. This project aims to assist in medical image analysis by accurately identifying and segmenting polyp regions.

---

## 🎯 Problem Statement
Manual detection of polyps in colonoscopy images is:<img width="255" height="256" alt="input" src="https://github.com/user-attachments/assets/5584db80-24f2-4278-beb5-bd9ac7cd3169" />

- Time-consuming  
- Prone to human error  

👉 This project builds a **deep learning-based solution** to automate the segmentation process.

---

## 🧠 Model Architecture
- U-Net (Encoder–Decoder CNN)
- Skip connections for better spatial information
- Designed specifically for biomedical image segmentation

---

## 📂 Dataset
- Colonoscopy image dataset with corresponding **ground truth masks**
- Preprocessing steps:
  - Image resizing  
  - Normalization  
  - Data augmentation  

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Resizing images  
- Normalizing pixel values  
- Data augmentation for robustness  

---

### 2. Model Implementation
- Built using:
  - Python  
  - TensorFlow / Keras  

---

### 3. Training
- Loss Function: Dice Loss  
- Optimizer: Adam  
- Dataset split:
  - Training  
  - Validation  
  - Testing  

---

### 4. Evaluation
Model performance evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1 Score  

---

## 📊 Results
| Metric | Training Set | Validation Set |
| :--- | :--- | :--- |
| **Accuracy (acc)** | 0.9849[cite: 1] | 0.9520[cite: 1] |
| **IOU** | 0.3825[cite: 1] | 0.3081[cite: 1] |
| **Loss (Binary Crossentropy)** | 0.1165[cite: 1] | 0.1707[cite: 1] |
| **Precision** | 0.9569[cite: 1] | 0.8105[cite: 1] |
| **Recall** | 0.9073[cite: 1] | 0.6871[cite: 1] |

- Achieved strong pixel-wise accuracy of 95.20% on the validation dataset.
- Demonstrated significant learning progress, reducing training loss from 0.5574 to 0.1165 over 42 epochs.
- Successfully improved precision to 81.05% on validation data, indicating a high rate of correct polyp pixel identification.
- Reached a Recall of 68.71% on the validation set, showing the model's ability to identify the majority of polyp regions.
- Optimized performance through learning rate management, with the optimizer successfully adapting from $1e-4$ down to $1e-8$ to refine weights.
- Maintained stable convergence after Epoch 32, with EarlyStopping ensuring the best weights were preserved before the validation loss plateaued.

---

## 📸 Output Samples

| Input Image | Ground Truth | Prediction |
|------------|-------------|------------|
| ![](sample/input.png) | ![](sample/groundtruth.png) | ![](sample/prediction.png) |

---

## 🛠 Tech Stack
- Programming Language: Python  
- Deep Learning Framework: TensorFlow and Keras
- Model Architecture: U-Net (Encoder-Decoder CNN)
- Optimization Algorithm: Adam Optimizer
- Data Processing: NumPy and TensorFlow tf.data
- API  Training : TensorBoard and CSVLogger
- Hardware Acceleration: NVIDIA GPU (/gpu:0)
- Model Management: Keras Callbacks (ModelCheckpoint, EarlyStopping, ReduceLROnPlateau)

---

## 🏆 Achievement
- Developed as part of academic/project work  
- Associated with **MNNIT project/certification**

  ![](certificate/mnnit_certificate_1.png)
👉 [View Certificate](certificate/shubhranshu_mnnit.pdf)

---

## 🚀 Applications
- Early detection of colorectal cancer  
- Computer-aided diagnosis systems  
- Medical image analysis  

---

## ⚠️ Limitations
- Performance depends on dataset quality  
- May struggle with complex or unclear images  

---

## 📌 Future Improvements
- Use advanced architectures (Attention U-Net, etc.)  
- Improve dataset size  
- Hyperparameter tuning  

---

## ⭐ Conclusion
This project demonstrates how deep learning can assist in **medical diagnostics** by automating polyp detection and improving accuracy.
