

---

# 🛳️ Titanic Dataset EDA – Survival Analysis

This project explores the famous Titanic dataset with a focus on **data profiling, univariate, bivariate, and multivariate analysis**, along with **outlier detection**. The goal is to uncover insights into the factors that influenced passenger survival.

---

## 📁 Project Structure

```
titanic-eda/
├── titanicdataset-eda.ipynb
├── images/
│   ├── age_distribution.png
│   ├── fare_boxplot.png
│   ├── pclass_survival_heatmap.png
│   └── correlation_heatmap.png
├── data/
│   └── train.csv
└── README.md
```

---

## 📊 Features of Analysis

### 1. 🧮 **Data Profiling**

* Types of variables
* Missing values
* Duplicates
* Errors
* Feature distributions

Example:

```python
df.info()
df.describe()
df.isnull().sum()
```

---

### 2. 📈 **Univariate Analysis**

Understand the distribution of each variable:

* Age distribution
* Fare distribution
* Categorical counts like Sex, Pclass, and Embarked

📸 *Visual Example:*

![Age Distribution](https://github.com/Wuodmadam/Kaggle-notebook-Titanic/blob/master/imputed%20age%20shot.png)

---

### 3. 🔁 **Bivariate Analysis**

Investigate relationships between pairs of features and survival.

* Survival vs Sex
* Survival vs Pclass
* Survival vs Embarked

📸 *Visual Example:*

![]()
```python
sns.catplot(x='Pclass', hue='Survived', col='Embarked', data=df, kind='count')
```

---

### 4. 🔀 **Multivariate Analysis**

Explore how **multiple variables interact** in relation to survival:

* Age, Pclass, and Fare combined
* Embarked location and class influence on survival

📸 *Example Output*:



---

### 5. ❗ **Outlier Detection**

Handled using visual and statistical techniques:

* Boxplots to detect outliers in `Fare`, `Age`, etc.
* Optionally removed or flagged for downstream modeling

📸 *Fare Outlier Plot:*



---

## 📌 Key Findings

* 🧍 **Sex**: Females had a significantly higher survival rate.
* 🧳 **Pclass**: Higher classes had better survival chances.
* 💰 **Fare**: Paying more often correlated with better chances of survival.
* 🧒 **Age**: Children (especially under 10) had higher survival than older passengers.

---

## 🧠 Technologies Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib
* Statsmodels

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/titanic-eda.git
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Launch the notebook:

   ```bash
   jupyter notebook titanicdataset-eda.ipynb
   ```

---

## 📂 Dataset Source

* [Kaggle Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)

---

## 🤝 Contributing

Contributions, feedback, or even better visuals are welcome!
Just open an issue or submit a pull request.

---

## 📄 License

MIT License

---


