# 🚀 Asteroid Hazard Classification

## 🌍 Overview

This project aims to classify asteroids based on their hazard potential using machine learning techniques. The dataset contains various asteroid features, and the model predicts whether an asteroid is potentially hazardous or not.

## 📂 Project Structure

- `asteroid_hazard_classification.py`: Main script for data processing, model training, and evaluation.
- `README.md`: Documentation of the project.

## 📊 Dataset

The dataset used in this project is from Kaggle: [NASA Nearest Earth Objects (1910-2024)](https://www.kaggle.com/datasets/ivansher/nasa-nearest-earth-objects-1910-2024/data). It includes features such as asteroid size, velocity, orbit details, and more. The target variable indicates whether the asteroid is hazardous (`True`) or not (`False`).

## 🔍 Preprocessing

- Applied **SMOTE** for balancing the dataset.
- Performed **feature scaling** using `StandardScaler`.
- Split the dataset into training and testing sets.

## 🤖 Model Training

The classification model used is **Random Forest Classifier**, which provided the best performance among tested models.

```python
from sklearn.ensemble import RandomForestClassifier

# Model training
model = RandomForestClassifier(class_weight='balanced', random_state=42)
model.fit(X_train_scaled, y_train)
```

## 🎯 Results

The final model achieved an accuracy of **95%** with balanced precision and recall, indicating a well-performing classifier.

### Confusion Matrix:

```
[[56152  2729]
 [ 3140 55981]]
```

## 🚀 How to Run on Google Colab

1. Open **Google Colab** and upload the script `asteroid_hazard_classification.py`.
2. Run the script in Colab cells.

Alternatively, you can create a new **Google Colab Notebook** and copy the script contents inside code cells.

## 📝 Future Improvements

- Experiment with other machine learning models like **XGBoost** or **LightGBM**.
- Optimize hyperparameters for better performance.
- Deploy the model as an API.

## 📬 Contact

For any questions or suggestions, feel free to reach out! ✉️

- **LinkedIn:** [Rawan Alalweet](https://www.linkedin.com/in/rawan-alalweet/)
- **Email:** rawan.alalweet@gmail.com


