# ❤️ Heart Disease Classification using Logistic Regression

A machine learning project that predicts the presence of heart disease using **Logistic Regression** with **feature standardization**, evaluated using accuracy, precision, recall, and a confusion matrix.

---

## 📁 Dataset

The project uses the **Heart Disease dataset** (`heart.csv`) with **303 records** and **14 features**, including:

| Feature | Description |
|---|---|
| `age` | Age of the patient |
| `sex` | Sex (1 = male, 0 = female) |
| `cp` | Chest pain type (0–3) |
| `trestbps` | Resting blood pressure |
| `chol` | Serum cholesterol |
| `fbs` | Fasting blood sugar > 120 mg/dl |
| `restecg` | Resting ECG results |
| `thalach` | Max heart rate achieved |
| `exang` | Exercise-induced angina |
| `oldpeak` | ST depression induced by exercise |
| `slope` | Slope of peak exercise ST segment |
| `ca` | Number of major vessels colored by fluoroscopy |
| `thal` | Thalassemia type |
| `target` | **1 = Heart disease, 0 = No heart disease** |

---

## 🔧 Tech Stack

- Python 3.x
- pandas
- scikit-learn
- seaborn

---

## 🚀 Workflow

1. **Load & Explore Data** — shape, dtypes, null check, class distribution
2. **Feature/Target Split** — `X` = all columns except `target`, `y` = `target`
3. **Train-Test Split** — 80/20 split with `random_state=42`
4. **Baseline Model** — Logistic Regression without scaling
5. **Standardization** — Applied `StandardScaler` (fit on train, transform on both)
6. **Model Retraining** — Logistic Regression on scaled features
7. **Evaluation** — Confusion matrix, accuracy, precision, recall

---

## 📊 Results

| Stage | Accuracy | Precision |
|---|---|---|
| Without Scaling | **88.5%** | 87.9% |
| With Standardization | 85.2% | 87.1% |

> Confusion Matrix (after scaling):
> ```
> [[25  4]
>  [ 5 27]]
> ```
> Recall: **84.4%**

---

## 📂 Project Structure
```
heart-disease-classification/
│
├── Logistic_regression.ipynb   # Main notebook
├── heart.csv                   # Dataset
└── README.md
```

---

## ▶️ How to Run
```bash
git clone https://github.com/your-username/heart-disease-classification-logistic-regression.git
cd heart-disease-classification-logistic-regression
pip install pandas scikit-learn seaborn
jupyter notebook Logistic_regression.ipynb
```

---

## 📌 Key Concepts Covered

- Binary classification
- Logistic Regression with `max_iter=1000`
- Feature standardization with `StandardScaler`
- Evaluation metrics: Accuracy, Precision, Recall, Confusion Matrix

---

## 📜 License
MIT
