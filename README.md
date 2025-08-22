 🔬 SmartPredict: Machine Learning for Early Diabetes Prediction  

## 📌 Overview  
Early detection of **diabetes** can save lives by preventing severe complications like heart disease, kidney failure, and nerve damage.  
This project compares **five machine learning algorithms** on the **Pima Indians Diabetes Dataset** to forecast diabetes:  

- 📈 Logistic Regression (LR)  
- 🌳 Decision Tree (DT)  
- 🌲 Random Forest (RF)  
- 👥 K-Nearest Neighbors (KNN)  
- 📊 Support Vector Machine (SVM)  

👉 **Key finding**: Random Forest achieved the highest performance, showing the strength of ensemble methods in healthcare prediction.  

---

## 📂 Dataset  
- **Source**: [Pima Indians Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  
- **Records**: 768 Pima Indian women  
- **Features**:  
  - Pregnancies  
  - Glucose  
  - Blood Pressure  
  - Skin Thickness  
  - Insulin  
  - BMI  
  - Diabetes Pedigree Function  
  - Age  
- **Target**: Diabetic (1) / Non-Diabetic (0)  

---

## ⚙️ Methodology  
1. **Data Preprocessing**  
   - Replaced invalid `0` values with mean values  
   - Standardized features using `StandardScaler`  
   - Train-test split (80/20)  

2. **Model Training**  
   - Implemented with `scikit-learn`  
   - 5-fold cross-validation for reliability  

3. **Evaluation Metrics**  
   - Accuracy (%)  
   - Confusion Matrix  
   - ROC Curve  
   - Feature Importance (Random Forest)  

---

## 📊 Results  

### 🔹 Cross-Validation Accuracy
| Algorithm            | Accuracy (%) |
|----------------------|--------------|
| 🌲 Random Forest     | **77.37**    |
| 📊 Support Vector Machine | 76.50    |
| 📈 Logistic Regression   | 76.06    |
| 👥 K-Nearest Neighbors   | 74.44    |
| 🌳 Decision Tree         | 72.80    |

---

### 🔹 Test Set Accuracy
| Algorithm            | Accuracy (%) |
|----------------------|--------------|
| 🌲 Random Forest     | **75.97**    |
| 📊 Support Vector Machine | 75.50    |
| 📈 Logistic Regression   | 75.32    |
| 🌳 Decision Tree         | 74.68    |
| 👥 K-Nearest Neighbors   | 69.48    |

✅ **Best Model**: Random Forest  

---

## 📈 Visualizations  
- 🔥 Correlation Heatmap of Features  
- 📊 Bar Plots of Accuracy  
- 🌀 Confusion Matrices for each model  
- 📉 ROC Curves (AUC Comparison)  
- 🌲 Feature Importance (Random Forest)  
- 📚 Learning & Calibration Curves  

---

## 🛠️ Tech Stack  
- **Language**: Python 3.9+  
- **Environment**: Jupyter Notebook / Google Colab  
- **Libraries**:  
  - `pandas`  
  - `numpy`  
  - `scikit-learn`  
  - `matplotlib`  
  - `seaborn`  

---

## 📂 Repository Structure  
├── data/
│ └── diabetes.csv # Dataset
├── notebooks/
│ └── diabetes_analysis.ipynb # Jupyter Notebook
├── results/
│ └── visualizations/ # Graphs & plots
├── README.md # Documentation
└── LICENSE # MIT License

yaml
Copy
Edit

---

## ✨ Key Takeaways  
- ✅ **Random Forest** performed best (highest accuracy & stability)  
- 📈 Logistic Regression = great **interpretability** for healthcare  
- ❌ KNN = weakest model, sensitive to scaling & noise  
- ⭐ Important predictors: **Glucose, BMI, Age**  

---

## 🔮 Future Work  
- Implement **Deep Learning models** (e.g., Neural Networks)  
- Handle **class imbalance** using SMOTE or weighted loss  
- Improve **explainability** of ensemble methods for clinicians  

---

## 👨‍💻 Author  
**Agha Wafa Abbas**  
- Lecturer, School of Computing, Arden University, UK  
- Lecturer, Pearson, London, UK  
- Lecturer, IVY College of Management Sciences, Pakistan  
- 📧 Email: awabbas@arden.ac.uk  

---

## 📜 Citation  
If you use this work, please cite:  

> Agha Wafa Abbas, *SmartPredict: A Comparative Exploration of Machine Learning for Early Diabetes Forecasting*  

---

## ⚖️ License  
This project is licensed under the **MIT License** – see the [LICENSE](./LICENSE) file for details. 
