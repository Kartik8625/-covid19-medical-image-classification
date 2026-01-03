# 🩺 COVID-19 Medical Image Classification using Machine Learning & Deep Learning

This project presents a **comprehensive medical image classification pipeline** for detecting **COVID-19, Normal, and Viral Pneumonia** cases from chest X-ray images.
Both **classical machine learning** and **deep learning (CNN)** approaches are implemented, evaluated, and compared.

---

## 📌 Project Overview

Early and accurate diagnosis of COVID-19 from chest X-ray images is critical in healthcare.
This project explores two complementary approaches:

1. **Classical Machine Learning**

   * Hand-crafted texture features (Haralick)
   * Traditional classifiers (QDA, Logistic Regression, Random Forest, etc.)

2. **Deep Learning**

   * Convolutional Neural Network (CNN)
   * End-to-end feature learning from raw images

The goal is to **compare performance, interpretability, and generalization** across approaches.

---

## 🗂️ Dataset

* **Source:** Public COVID-19 Chest X-ray dataset (via Kaggle / IBM CognitiveClass)
* **Classes:**

  * Covid
  * Normal
  * Viral Pneumonia
* **Data Split:**

  * Training set
  * Test/Validation set

⚠️ **Note:**
The dataset is **not included** in this repository due to size constraints.

---

## 🧠 Methodology

### 1️⃣ Classical Machine Learning Pipeline

* Image preprocessing (grayscale, resizing)
* Feature extraction using **Haralick texture descriptors**
* Feature scaling with `StandardScaler`
* Model training using:

  * Logistic Regression
  * K-Nearest Neighbors
  * Support Vector Machines
  * Random Forest
  * **Quadratic Discriminant Analysis (QDA)** (best performer)
* Evaluation using:

  * Accuracy
  * Precision, Recall, F1-Score
  * Confusion Matrix

---

### 2️⃣ Deep Learning Pipeline (CNN)

* Data loading using `ImageDataGenerator`
* On-the-fly data augmentation
* CNN architecture with:

  * Convolutional layers
  * Max-Pooling
  * Dropout for regularization
* Training using TensorFlow / Keras
* Evaluation using:

  * Accuracy & Loss curves
  * Classification Report
  * Confusion Matrix

---

## 📊 Results Summary

| Approach      | Best Model              | Performance                  |
| ------------- | ----------------------- | ---------------------------- |
| Classical ML  | QDA (Haralick features) | ~83% test accuracy           |
| Deep Learning | CNN                     | **~92% validation accuracy** |

### 🔍 Key Observations

* Classical ML performs well with handcrafted texture features.
* CNN significantly improves performance by learning spatial patterns directly from images.
* CNN shows better generalization on complex classes like **Viral Pneumonia**.

---

## 🧪 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix (class-wise error analysis)

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries & Frameworks:**

  * TensorFlow / Keras
  * Scikit-learn
  * NumPy, Pandas
  * Matplotlib, Seaborn
  * Mahotas (Haralick features)
* **Environment:** Google Colab
* **Version Control:** Git & GitHub

---

## 📁 Repository Structure

```
covid19-medical-image-classification/
│
├── healthcare_ml_classification.ipynb   # Main notebook (ML + CNN)
├── README.md                            # Project documentation
├── requirements.txt                    # Dependencies
├── models/
│   └── .gitkeep                        # Placeholder (model not uploaded)
└── .gitignore
```

---

## 💾 Trained Model

The trained CNN model (`.keras` file) is **not included** in this repository due to GitHub file size limits.

You can:

* Reproduce the model by running the notebook end-to-end in Google Colab
* Or host the model externally (Google Drive) and link it here if needed

---

## 🚀 How to Run the Project

1. Clone the repository
2. Open `healthcare_ml_classification.ipynb` in **Google Colab**
3. Install dependencies (if required)
4. Download and place the dataset in the expected directory structure
5. Run all cells sequentially

## ▶️ Run on Google Colab

You can run this project directly on Google Colab without any local setup.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/Kartik8625/-covid19-medical-image-classification/blob/main/healthcare_ml_classification.ipynb
)


---

## 🧾 Conclusion

This project demonstrates a **full-stack machine learning workflow** for medical image classification, covering:

* Feature engineering
* Model comparison
* Deep learning implementation
* Proper evaluation and reporting

By combining **classical ML** and **CNN-based deep learning**, the project highlights the strengths and trade-offs of both approaches in real-world healthcare applications.

---

## 👤 Author

**Kartik Inamdar**
Aspiring Data Analyst / Machine Learning Engineer
GitHub: [https://github.com/Kartik8625](https://github.com/Kartik8625)

---

