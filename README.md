# Handwritten Digit Classification using KNN ✍️🧠

## Task Information
This task focuses on implementing a **K-Nearest Neighbors (KNN)** model to classify handwritten digits (0–9).  
The objective is to understand distance-based learning and evaluate model performance using different values of K.

---

## Objective 🎯
- Build a KNN classifier for handwritten digit recognition  
- Analyze the impact of different K values  
- Evaluate the model using accuracy and confusion matrix  

---

## Dataset Information 📊
- Dataset: Scikit-learn Digits Dataset (`load_digits`)
- Total samples: 1797
- Number of classes: 10 (digits 0–9)
- Image size: 8 × 8 grayscale
- Features per sample: 64 (flattened pixel values)

Each image is converted into a numerical feature vector before training.

---

## Tools & Technologies 🛠️
- Python
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

---

## Data Preprocessing ⚙️
- Dataset is split into training (80%) and testing (20%)
- Feature scaling is applied using `StandardScaler`
- Scaling is essential because KNN relies on Euclidean distance

---

## Model Description 🧩
- Algorithm: K-Nearest Neighbors (KNN)
- Learning type: Supervised learning
- Distance metric: Euclidean distance
- Initial K value: 3
- Additional K values tested: 5, 7, 9

The optimal K value is selected based on accuracy comparison.

---

## Model Training 🚀
- The model is trained using scaled training data
- For each test sample, distances to nearest neighbors are calculated
- The predicted class is determined using majority voting

---

## Model Evaluation 📈
The model is evaluated using:
- Accuracy score
- Accuracy vs K-value graph
- Confusion matrix
- Visualization of test images with predicted labels

---

## Results & Observations ✅
- The model achieves high accuracy on the digits dataset
- Smaller K values are sensitive to noise
- Larger K values provide smoother decision boundaries
- Feature scaling significantly improves performance

---

## Conclusion 🧠
KNN proves to be an effective algorithm for handwritten digit classification when proper preprocessing and parameter tuning are applied. This project demonstrates the importance of distance metrics, scaling, and hyperparameter selection in machine learning.

---

## Applications 💡
- Handwritten digit recognition
- Optical Character Recognition (OCR)
- Educational ML projects
- Baseline comparison for advanced models (SVM, CNN)
