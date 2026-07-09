# ✍️ Handwritten Character Recognition using CNN
### CodeAlpha Internship — Task 3

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.20-FF6F00?style=for-the-badge&logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-D00000?style=for-the-badge&logo=keras)
![Accuracy](https://img.shields.io/badge/Test%20Accuracy-99.15%25-success?style=for-the-badge)
![Dataset](https://img.shields.io/badge/Dataset-MNIST-blueviolet?style=for-the-badge)

---

## 📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** to recognize handwritten digits from the **MNIST dataset**.

The model learns distinctive visual patterns such as edges, curves, and strokes to accurately classify digits **0–9**. It demonstrates the effectiveness of CNNs for image classification tasks and achieves **99.15% test accuracy**.

---

## 🎯 Objective

Develop a deep learning model capable of accurately recognizing handwritten digits using the MNIST dataset while applying CNN architecture, dropout regularization, and early stopping for improved performance.

---

## 🖼 Dataset

**MNIST Handwritten Digit Dataset**

- 📚 60,000 Training Images
- 🧪 10,000 Testing Images
- 🖼 Image Size: **28 × 28 pixels**
- 🔢 Classes: **10 (Digits 0–9)**

---

# 🏗 Model Architecture

```
Input (28 × 28 × 1)

│

├── Conv2D (32 Filters, 3×3, ReLU)
├── MaxPooling2D

├── Conv2D (64 Filters, 3×3, ReLU)
├── MaxPooling2D

├── Conv2D (64 Filters, 3×3, ReLU)

├── Flatten

├── Dense (128, ReLU)

├── Dropout (0.5)

└── Dense (10, Softmax)
```

### 📊 Total Parameters

**130,890 Trainable Parameters**

---

# 🚀 Training Configuration

| Parameter | Value |
|-----------|--------|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Metric | Accuracy |
| Batch Size | 64 |
| Epochs | 20 |
| Early Stopping | Enabled |
| Restore Best Weights | Yes |

---

# 📈 Results

| Metric | Value |
|---------|--------|
| ✅ Test Accuracy | **99.15%** |
| 📉 Test Loss | **0.0310** |
| 🛑 Early Stopping | Epoch **10** |
| ⭐ Best Model | Epoch **7** |

---

# 📊 Performance Highlights

- ✅ Achieved **99.15% Test Accuracy**
- 🎯 Excellent generalization on unseen images
- 🚀 Early stopping prevented overfitting
- 🔥 Stable convergence during training
- 📉 Very low test loss of **0.0310**

---

# 🔍 Key Findings

### ✅ Best Performing Digit

**Digit 1**

- Precision: **1.00**
- Recall: **1.00**
- F1-Score: **1.00**

Perfect classification with zero missed predictions.

---

### ⚠ Most Challenging Digit

**Digit 7**

- **21 misclassified images**
- Mainly confused due to similarities in handwritten styles.

---

# 🛠 Tech Stack

- 🐍 Python
- 🧠 TensorFlow 2.20
- 🔥 Keras
- 🔢 NumPy
- 📊 Matplotlib
- 📈 Scikit-learn

---


# ▶️ How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/Handwritten-Character-Recognition.git
```

### 2️⃣ Navigate

```bash
cd Handwritten-Character-Recognition
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run

```bash
python handwritten_character_recognition.py
```

or open

```text
handwritten_character_recognition.ipynb
```

---


# 📌 Future Improvements

- ✅ Handwritten digit prediction from custom images
- 📷 Real-time digit recognition using webcam
- ☁ Deploy with Streamlit or Flask
- 📱 Mobile-friendly digit recognition interface
- 🔍 Hyperparameter tuning for even better performance

---

# 🎓 Learning Outcomes

Through this project, I gained hands-on experience with:

- Convolutional Neural Networks (CNNs)
- Image preprocessing
- Deep learning model training
- Early stopping and dropout regularization
- Performance evaluation using classification metrics
- TensorFlow & Keras workflows

---

# 📜 Internship

**CodeAlpha Internship**

**Task 3 — Handwritten Character Recognition**

---

# ⭐ Acknowledgements

- TensorFlow
- Keras
- MNIST Dataset
- CodeAlpha Internship Program

---

## 👩‍💻 Author

**Virakshi Dhawar**

- 💼 Computer Science Engineering Student
- 🤖 AI | Machine Learning | Full Stack Development
- 🌟 Passionate about building intelligent applications

---

## ⭐ If you found this project useful, don't forget to star the repository!
```

## How to Run
1. Open `.ipynb` in Google Colab
2. Enable GPU: Runtime → Change runtime type → T4 GPU
3. Run all cells top to bottom
4. Training completes in ~30 seconds per epoch

