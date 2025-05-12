# 🚗 Vehicle Price Prediction Using Deep Learning

This project predicts the prices of vehicles based on key features using a deep learning regression model built with TensorFlow and Keras.

---

## 📌 Project Overview

In the growing market of used and new vehicles, accurate pricing is crucial for buyers and sellers. This project builds a regression model to predict vehicle prices based on structured tabular data like make, model, mileage, fuel type, and more.

---

## 📸 App View 
| Web View                          | Another Features                 |
| --------------------------------- | -------------------------------- | 
![image](https://github.com/user-attachments/assets/635f8864-e9b2-4a98-81fe-809c39eb2fa3)|![image](https://github.com/user-attachments/assets/8cff8d3b-02dd-4b06-9c8c-84b8880f530b)|

---
## 🎯 Project Goal

- Predict vehicle prices using a deep learning model.
- Handle categorical and numerical data effectively.
- Evaluate model performance using Mean Squared Error.
- Provide a clean pipeline from data preprocessing to model evaluation.

---

## 📂 Dataset Overview

- **File**: `dataset.csv`
- **Size**: Tabular dataset with multiple vehicle features.
- **Target Column**: `price`
- **Preprocessing**:
  - Missing value handling (`fillna`, `dropna`)
  - Label Encoding for categorical variables
  - Standard Scaling for numerical features

---

## 🛠️ Tech Stack

| Component              | Tools/Libraries                          |
|------------------------|------------------------------------------|
| Language               | Python                                   |
| Data Manipulation      | pandas, numpy                            |
| Visualization          | matplotlib, seaborn                      |
| Preprocessing          | scikit-learn (LabelEncoder, StandardScaler) |
| Modeling               | TensorFlow, Keras                        |
| Model Saving           | joblib                                   |

---

## 🧪 Model Architecture

```python
model = Sequential([
    Dense(128, activation='relu', input_shape=(X.shape[1],)),
    Dropout(0.2),
    Dense(64, activation='relu'),
    Dropout(0.1),
    Dense(1)  # Output layer
])
model.compile(optimizer='adam', loss='mse')
````

---

## 🔄 Training

```python
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
model.fit(X_train, y_train, epochs=50, validation_data=(X_test, y_test))
```

---

## 📊 Results

* Loss function: Mean Squared Error
* Good convergence across epochs
* Robust predictions on unseen test data

---

## 💾 Saving the Model

```python
joblib.dump(scaler, 'scaler.pkl')
model.save('vehicle_price_model.h5')
```

---

## ✅ Conclusion

This model shows promising results in vehicle price prediction. Future improvements could involve:

* Feature engineering
* Handling outliers
* Compared with tree-based models like XGBoost or LightGBM

---

## 📎 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author
For queries or collaborations, feel free to connect:  
<p align="center">
  <a href="https://www.linkedin.com/in/aritramukherjeeofficial/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="https://x.com/AritraMofficial" target="_blank">
    <img src="https://img.shields.io/badge/Twitter-%231DA1F2.svg?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter">
  </a>
  <a href="https://www.instagram.com/aritramukherjee_official/?__pwa=1" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
  <a href="https://leetcode.com/u/aritram_official/" target="_blank">
    <img src="https://img.shields.io/badge/LeetCode-%23FFA116.svg?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode">
  </a>
  <a href="https://github.com/AritraOfficial" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-%23181717.svg?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://discord.com/channels/@me" target="_blank">
    <img src="https://img.shields.io/badge/Discord-%237289DA.svg?style=for-the-badge&logo=discord&logoColor=white" alt="Discord">
  </a>
  <a href="mailto:aritra.work.official@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Email-%23D14836.svg?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>


--- 

Feel free to reach out for collaboration or questions!


