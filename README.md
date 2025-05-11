# 🚗 Vehicle Price Prediction Using Deep Learning

This project predicts the prices of vehicles based on key features using a deep learning regression model built with TensorFlow and Keras.

---

## 📌 Project Overview

In the growing market of used and new vehicles, accurate pricing is crucial for buyers and sellers. This project builds a regression model to predict vehicle prices based on structured tabular data like make, model, mileage, fuel type, and more.

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
* Comparing with tree-based models like XGBoost or LightGBM

---

## 📎 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Aritra Mukherjee**
Feel free to reach out for collaboration or questions!


