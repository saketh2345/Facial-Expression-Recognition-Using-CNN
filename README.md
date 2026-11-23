# Facial Expression Recognition Using Deep Learning

## 📌 Project Overview

This project implements a Facial Expression Recognition (FER) system using deep learning and machine learning techniques. It detects human facial expressions from images and classifies them into seven emotion categories using the CK+ (Extended Cohn-Kanade) dataset.

The project compares three classification approaches to identify the best-performing model.

## 🎯 Objectives

- Recognize human facial expressions automatically.
- Classify facial images into seven emotion categories.
- Compare CNN and transfer learning approaches.
- Evaluate models using accuracy, F1-score, and confusion matrices.
- Improve generalization using subject-independent cross-validation.

## 😊 Emotion Classes

The model recognizes seven facial expressions:

1. Anger
2. Contempt
3. Disgust
4. Fear
5. Happy
6. Sad
7. Surprise

## 🧠 Models Implemented

The project evaluates three classification methods:

| Model | Held-out Accuracy |
|---|---:|
| ResNet-18 Original Head | 93.27% |
| ResNet-18 + RBF-SVM | **95.11%** |
| ResNet-18 + Logistic Regression | 93.58% |

**Best Model: ResNet-18 Features + RBF-SVM (95.11%)**

## 📂 Dataset

**CK+ (Extended Cohn-Kanade) Dataset**

- 327 peak-frame images
- 118 subjects
- 7 emotion categories

The dataset is downloaded using KaggleHub:

`shawon10/ckplus`

## ⚙️ Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- KaggleHub
- PIL

## 🔍 Methodology

1. Download and load the CK+ dataset.
2. Extract peak facial expression frames.
3. Preprocess and resize images to 128 × 128.
4. Apply image augmentation.
5. Split data using Stratified Group K-Fold cross-validation.
6. Train and evaluate ResNet-18.
7. Extract deep features from ResNet-18.
8. Train SVM and Logistic Regression classifiers.
9. Compare classification performance.
10. Generate confusion matrices and evaluation results.

## 📊 Results

The experimental results show that ResNet-18 feature extraction combined with an RBF-SVM classifier achieved the highest held-out accuracy.

| Evaluation | Result |
|---|---:|
| ResNet-18 | 93.27% |
| RBF-SVM | 95.11% |
| Logistic Regression | 93.58% |

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/facial-expression-recognition.git
cd facial-expression-recognition
```

Install dependencies:

```bash
pip install torch torchvision numpy pandas matplotlib scikit-learn pillow kagglehub
```

## ▶️ Run the Project

1. Open the Jupyter Notebook.
2. Run it using Google Colab or Jupyter Notebook.
3. Download the CK+ dataset.
4. Execute the notebook cells in order.
5. View the model comparison and confusion matrices.

## 📈 Evaluation Metrics

- Accuracy
- Macro F1-score
- Classification Report
- Confusion Matrix
- Five-fold subject-independent evaluation

## 🔮 Future Improvements

- Implement real-time facial expression recognition using a webcam.
- Improve performance with additional facial expression datasets.
- Develop a user-friendly graphical interface.
- Optimize the model for real-time applications.
- Explore additional CNN architectures.

## 👨‍💻 Author

**Your Name**

## 📜 License

This project is intended for educational and research purposes.
