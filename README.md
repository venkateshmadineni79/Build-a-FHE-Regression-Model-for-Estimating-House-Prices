# FHE Regression Model for Estimating Housing Prices

This project demonstrates a secure and privacy-preserving approach to predicting housing prices using a deep learning regression model combined with Fully Homomorphic Encryption (FHE). The model is trained on plaintext data using TensorFlow and deployed for encrypted inference using the TenSEAL library. The encryption scheme used is CKKS, allowing computations to be performed directly on encrypted data without decrypting it, thus maintaining data confidentiality throughout the prediction process.

---

## 📌 Project Task

This project trains a regression model in plaintext using TensorFlow and integrates it with OpenFHE library for encrypted inference using the CKKS scheme. Model weights remain plaintext, while inputs and outputs are encrypted to ensure user privacy.  

---

## 📊 Dataset

The dataset used in this project comes from the [FHERMA Challenge](https://fherma.io/challenges/676035a7890eef39561cf7c9/overview).  
It includes two CSV files:
- `X_train.csv`: Contains 13 numerical input features per sample such as average rooms, household income, and population.
- `y_train.csv`: Contains the corresponding target housing prices.


---

## 📁 Project Structure

```
fhe-regression/
├── data/       # Input datasets (X_train.csv, y_train.csv)
├── models/     # Trained model file (best_dnn_model.keras)
├── notebooks/  # Jupyter notebook (FHE_Regression_Model.ipynb)
├── reports/    # Report PDF 
```

---

## 🚀 How to Run

1. Open `notebooks/FHE_Regression_Model.ipynb`
2. Load and preprocess the dataset
3. Train a regression model on plaintext data
4. Save the model
5. Use TenSEAL to:
   - Encrypt input samples using CKKS
   - Run encrypted inference
   - Decrypt results and view predictions

---

## 📦 Dependencies

Install required packages using:

```bash
pip install -r requirements.txt
```

Key libraries used:
- `tensorflow` for training the deep learning model
- `scikit-learn` for preprocessing and metrics
- `pandas` and `numpy` for data handling
- `TenSEAL` for encrypted inference

---

## 📈 Model Evaluation

After training, the model is evaluated using:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R² Score

---

## 🔐 Why FHE?

Fully Homomorphic Encryption (FHE) enables secure computations on encrypted data. In this project, users can submit encrypted housing features and receive encrypted predictions — the server never sees the plaintext data or results, ensuring full data privacy.

---

## 📄 License

MIT License — see `LICENSE` file.