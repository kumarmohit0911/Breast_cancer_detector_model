# 🧠 Breast Cancer Detection using Deep Learning (MLP/ANN)

This project focuses on building a deep learning model using Multi-Layer Perceptron (MLP) to detect breast cancer based on cell features from the **Breast Cancer Wisconsin Dataset**. No traditional ML models like Logistic Regression or Random Forest were used — this is entirely deep learning-based.

---

## 📂 Dataset

- **Source**: [UCI Breast Cancer Wisconsin Dataset](https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(original))
- **Rows**: 699
- **Features**: 9 predictive features + 1 target class
- **Target**: `class`  
  - `2`: Benign  
  - `4`: Malignant

---

## 🔍 Features Used

- `clump_thickness`
- `size_uniformity`
- `shape_uniformity`
- `marginal_adhesion`
- `epithelial_size`
- `bare_nucleoli` (cleaned)
- `bland_chromatin`
- `normal_nucleoli`
- `mitoses`

---

## 🧼 Data Preprocessing

- Handled missing values in `bare_nucleoli` (`?` replaced and converted to float)
- Normalized feature values using `MinMaxScaler`
- Target class converted to binary:  
  - `0` → Benign  
  - `1` → Malignant

---

## 🧠 Model Architecture (MLP)

- Input Layer: 9 neurons
- Hidden Layers: 2 layers with ReLU activation
- Output Layer: 1 neuron with sigmoid activation
- Loss Function: Binary Crossentropy
- Optimizer: Adam
- Epochs: 100

---

## ✅ Results

| Metric               | Value      |
|----------------------|------------|
| **Accuracy**         | 96.57%     |
| **Mean Absolute Error** | 0.034     |
| **Validation Accuracy** | 0.9623  (may vary slightly by run) |

---

## 📦 Tech Stack

- Python
- pandas, NumPy
- scikit-learn
- TensorFlow & Keras
- Google Colab

---

## 📌 Key Learnings

- Applied real-world data cleaning on medical data
- Designed and trained an MLP for binary classification
- Understood importance of preprocessing and feature engineering in DL

---

## 📸 Demo

Add screenshots of graphs or model summary (optional)

---

## 📁 How to Run

```bash
# Clone the repo
git clone https://github.com/yourusername/breast-cancer-detection-ann.git
cd breast-cancer-detection-ann

# Run on Colab or Jupyter
