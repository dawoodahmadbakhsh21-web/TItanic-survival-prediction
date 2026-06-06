# 🚢 Titanic Survival Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Sklearn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![Kaggle](https://img.shields.io/badge/Dataset-Kaggle-20BEFF)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

Predicting survival on the Titanic using machine learning. This project covers end-to-end ML pipeline: EDA, feature engineering, model training, and evaluation.

---

## 📊 Dataset
- **Source:** [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic)
- **Size:** 891 passengers (training set)
- **Target:** Survived (0 = No, 1 = Yes)

---

## 🔍 Key Insights from EDA
- **Women** had a much higher survival rate than men (~74% vs ~19%)
- **1st class** passengers survived more than 2nd and 3rd class
- **Children** (Age < 12) had higher survival rates
- **Higher fare** positively correlated with survival

---

## ⚙️ Feature Engineering
| Feature | Description |
|---------|-------------|
| `FamilySize` | SibSp + Parch + 1 |
| `IsAlone` | 1 if traveling alone |
| `Title` | Extracted from Name (Mr, Mrs, Miss, Master, Rare) |
| `AgeBand` | Age grouped into Child / Teen / Adult / Middle / Senior |

---

## 🤖 Model Comparison
| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| Logistic Regression | 0.7989 | 0.8574 |
| Random Forest ✅ | 0.8212 | 0.8409 |
| Gradient Boosting | 0.8156 | 0.8177 |
| SVM | 0.6201 | 0.6921 |

**Best Model: Random Forest** with Accuracy = `0.8212` and ROC-AUC = `0.8409`

---

## 📈 Visualizations

### Survival Analysis
![Survival](eda_survival.png)

### Age & Fare Distribution
![Age Fare](eda_age_fare.png)

### Feature Importance
![Feature Importance](feature_importance.png)

### Model Comparison
![Model Comparison](model_comparison.png)

---

## 🗂️ Project Structure
```
titanic-survival-prediction/
├── titanic_survival_prediction.ipynb
├── titanic_project/
│   ├── titanic_model.pkl
│   └── feature_columns.json
├── eda_survival.png
├── eda_age_fare.png
├── eda_heatmap.png
├── model_comparison.png
├── best_model_eval.png
├── feature_importance.png
└── README.md
```

## 🚀 How to Run
1. Clone the repo
2. Open `titanic_survival_prediction.ipynb` in Google Colab
3. Run all cells top to bottom

## 🛠️ Tech Stack
- Python 3.10
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-Learn (Logistic Regression, Random Forest, Gradient Boosting, SVM)

## 👤 Author
**Dawood Ahmad** — [GitHub](https://github.com/yourusername) | [LinkedIn](https://linkedin.com/in/dawood-ahmad-b46641361)
