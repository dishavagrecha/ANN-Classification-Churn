
# 🧠 Customer Churn Prediction (ANN)

This project predicts whether a customer is likely to churn using an Artificial Neural Network (ANN) built with TensorFlow/Keras.

## 📊 Dataset
- [Churn Modeling Dataset](https://www.kaggle.com/datasets/shubhendra7/churn-modelling)  
- Contains customer demographics, account information, and churn labels.

## 🔧 Preprocessing
- Dropped irrelevant columns: `RowNumber`, `CustomerId`, `Surname`
- Encoded categorical features:
  - `Gender` → Label Encoding
  - `Geography` → One-Hot Encoding
- Standardized numerical features using `StandardScaler`

## 🧠 Model Architecture
- ANN built using `tensorflow.keras.models.Sequential`
- Hidden Layers: ReLU activation
- Output Layer: Sigmoid activation
- Loss: Binary Cross-Entropy  
- Optimizer: Adam  
- Metrics: Accuracy

## ✅ Performance
- **Test Accuracy:** 87.48%

## 🗃️ Artifacts
- Pickled encoders and scaler (`.pkl`)
- Trained ANN model saved as `.h5`

## 📈 Future Work
- Add model explainability (SHAP/LIME)
- Deploy using Flask or Streamlit
