# 🎙️ Emotion Recognition from Speech
### CodeAlpha Internship — Task 2

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?style=for-the-badge&logo=tensorflow)
![Librosa](https://img.shields.io/badge/Librosa-Audio%20Processing-blueviolet?style=for-the-badge)
![Accuracy](https://img.shields.io/badge/Test%20Accuracy-71.88%25-success?style=for-the-badge)
![Dataset](https://img.shields.io/badge/Dataset-RAVDESS-green?style=for-the-badge)

---

# 📌 Project Overview

This project builds a **Speech Emotion Recognition (SER)** system that classifies human emotions from speech audio using **Mel-Frequency Cepstral Coefficients (MFCCs)** and a **Deep Neural Network (DNN)**.

The model learns acoustic patterns from voice recordings to recognize eight different emotional states, demonstrating the application of deep learning in speech processing and human-computer interaction.

---

# 🎯 Objective

Develop a deep learning model capable of recognizing human emotions from speech audio by extracting meaningful audio features and classifying them into predefined emotional categories.

---

# 🎧 Dataset

**RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**

- 🎭 24 Professional Actors
- 🎤 Speech-Only Audio
- 📊 Total Samples: **1,440**
- 🎯 Emotion Classes: **8**

### Emotion Categories

- 😐 Neutral
- 😌 Calm
- 😀 Happy
- 😢 Sad
- 😠 Angry
- 😨 Fearful
- 🤢 Disgust
- 😲 Surprised

---

# 🏗 Model Architecture

```
Audio Input

│

├── MFCC Feature Extraction
│      (40 Coefficients)
│
├── Mean Pooling
│
├── Dense (256, ReLU)
│
├── Dropout
│
├── Dense (128, ReLU)
│
├── Dropout
│
└── Dense (8, Softmax)
```

### 📊 Total Parameters

**44,424 Trainable Parameters**

---

# 🚀 Training Configuration

| Parameter | Value |
|-----------|--------|
| Feature Extraction | MFCC (40 Coefficients) |
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Metric | Accuracy |
| Early Stopping | Enabled |
| Dataset | RAVDESS |

---

# 📈 Results

| Metric | Value |
|---------|--------|
| ✅ Test Accuracy | **71.88%** |
| 📉 Test Loss | **0.8101** |

---

# 📊 Performance Highlights

- ✅ Successfully classified **8 speech emotions**
- 🎙 MFCC features effectively captured emotional speech characteristics
- 🛑 Early stopping reduced unnecessary training and helped limit overfitting
- 🚀 Achieved solid performance on a relatively small emotional speech dataset

---

# 🔍 Key Findings

### 🌟 Best Performing Emotions

- 😨 **Fearful** — Recall: **0.87**
- 😠 **Angry** — Recall: **0.79**

These emotions exhibit distinctive vocal patterns, making them easier for the model to recognize.

---

### ⚠ Most Confused Emotion Pairs

- 😐 Neutral ↔ 😌 Calm
- 😢 Sad ↔ 😨 Fearful

These emotions share similar acoustic characteristics, making them challenging to distinguish, even for human listeners.

---

### 📌 Model Insights

- Training Accuracy: **~94%**
- Validation Accuracy: **~72%**

The gap indicates **moderate overfitting**, which is expected due to the relatively small dataset size (**1,152 training samples**). Despite this, the model demonstrates good generalization for speech emotion recognition.

---

# 🛠 Tech Stack

- 🐍 Python
- 🎵 Librosa
- 🧠 TensorFlow / Keras
- 📊 Scikit-learn

---

# ▶️ How to Run

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/Emotion-Recognition-from-Speech.git
```

### 2️⃣ Navigate to the Project

```bash
cd Emotion-Recognition-from-Speech
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Project

```bash
python emotion_recognition.py
```

or simply open the notebook in **Google Colab** and run all cells.

> **The RAVDESS dataset is automatically downloaded from Zenodo during execution.**

---

---

# 📌 Future Improvements

- 🎤 Real-time speech emotion recognition
- 🌐 Deploy using Streamlit or Flask
- 🧠 Experiment with CNN, LSTM, or Transformer architectures
- 🎧 Incorporate additional audio features such as Chroma and Mel Spectrograms
- 📊 Train on larger and more diverse emotional speech datasets

---

# 🎓 Learning Outcomes

Through this project, I gained practical experience with:

- Speech Emotion Recognition (SER)
- Audio Signal Processing
- MFCC Feature Extraction
- Deep Neural Networks
- Model Evaluation using Classification Metrics
- Overfitting Analysis and Early Stopping
- TensorFlow/Keras & Librosa workflows

---

# 📜 Internship

**CodeAlpha Internship**

**Task 2 — Emotion Recognition from Speech**

---

# ⭐ Acknowledgements

- RAVDESS Dataset
- TensorFlow
- Librosa
- Scikit-learn
- CodeAlpha Internship Program

---

## 👩‍💻 Author

**Virakshi Dhawar**

- 💼 Computer Science Engineering Student
- 🤖 AI | Machine Learning | Full Stack Development
- 🌟 Passionate about building intelligent applications

---

## ⭐ If you found this project useful, don't forget to star the repository!
