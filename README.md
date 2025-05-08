# FHE Regression Model for Estimating Housing Prices

This project demonstrates a secure way to estimate housing prices using a deep learning regression model under Fully Homomorphic Encryption (FHE). The model is trained in plaintext using TensorFlow, and used in encrypted inference via OpenFHE.

---

## 📁 Project Structure

```
fhe-regression/
├── data/       # Input datasets (X_train.csv, y_train.csv)
├── models/     # Trained model file (best_dnn_model.keras)
├── notebooks/  # Jupyter notebook (FHE_Regression_Model.ipynb)
├── reports/    # Report PDF and assignment brief
```

---

## 🚀 How to Run

1. Open `notebooks/FHE_Regression_Model.ipynb`
2. Train the model on housing data
3. Run encrypted inference using OpenFHE
4. Decrypt the output locally

---

## 📦 Dependencies

See `requirements.txt`. To install:

```bash
pip install -r requirements.txt
```

---

## 🔐 Why FHE?

FHE ensures user privacy by allowing encrypted input and output without revealing data to the server.

---

## 📄 License

MIT License — see `LICENSE` file.