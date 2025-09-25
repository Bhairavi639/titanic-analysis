# Titanic Survival Prediction 🚢⚓  

## 📌 Project Overview  
This project uses the famous Titanic dataset to **predict passenger survival** using **Machine Learning**.  
We perform data cleaning, feature engineering, visualization, and modeling with **Logistic Regression**.  

The goal is to explore the data, understand the important features (like Sex, Age, Pclass, Fare, etc.), and build a predictive model that estimates the probability of survival.  

---

## 📂 Dataset  
- Dataset used: `Titanic-Dataset.csv`  
- Size: **891 rows × 12 columns**  
- Target column: **Survived (0 = Did not survive, 1 = Survived)**  

### Key Features  
- `Pclass` → Passenger Class (1 = First, 2 = Second, 3 = Third)  
- `Sex` → Gender (male/female)  
- `Age` → Age in years  
- `SibSp` → Number of siblings/spouses aboard  
- `Parch` → Number of parents/children aboard  
- `Fare` → Ticket fare  
- `Embarked` → Port of embarkation (S, C, Q)  

---

## 🛠️ Steps in the Project  

### 1. **Data Preprocessing**  
- Removed irrelevant columns: `PassengerId`, `Name`, `Ticket`, `Cabin`  
- Filled missing values:  
  - `Age` → filled with median  
  - `Embarked` → filled with mode (most frequent value)  
- Encoded categorical variables using **LabelEncoder**  

### 2. **Exploratory Data Analysis (EDA)**  
- Count plots for categorical variables (`Sex`, `Embarked`)  
- Histograms & boxplots for numerical variables (`Age`, `Fare`, etc.)  
- Pie chart of gender distribution  
- Strip plot of `Fare vs Embarked`  

### 3. **Modeling**  
- **Model Used** → Logistic Regression  
- Train/Test Split: 80/20  
- Model Accuracy: **~81%**  
- Predictions made on test set  
- Probability predictions available (`predict_proba`)  

### 4. **Evaluation**  
- Accuracy score on test set: **0.81**  
- Predicted vs actual values compared  
- Survival probabilities visualized  

---

## 📊 Visualizations  
- Histograms & Boxplots for numerical features  
- Count plot for `Embarked`  
- Pie chart of `Sex` distribution  
- Strip plot of `Fare` vs `Embarked`  

---

## 📦 Requirements  
Install the dependencies before running:  

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## ▶️ How to Run  
1. Clone/download this repository.  
2. Place `Titanic-Dataset.csv` in the project folder.  
3. Run the Jupyter Notebook / Python script:  

```bash
python titanic_model.py
```

4. Model will be trained and evaluated, accuracy printed, and plots displayed.  

---

## 🚀 Future Improvements  
- Try other ML models: Random Forest, SVM, Gradient Boosting, XGBoost  
- Perform feature scaling (e.g., StandardScaler)  
- Hyperparameter tuning with GridSearchCV  
- Deploy model with Flask/Streamlit  

---

