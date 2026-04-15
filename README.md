# 🏡 Housing Price Prediction

This project explores a housing dataset and builds a machine learning model to predict median house values based on demographic and geographic features.

The focus is on combining **exploratory data analysis (EDA)** with a clean modeling pipeline to understand what drives housing prices and establish a strong baseline model.

---

## 🚀 Project Overview

This notebook walks through an end-to-end workflow:

* Data loading and exploration
* Visualization of feature distributions and relationships
* Handling missing data
* Encoding categorical variables
* Building a preprocessing + modeling pipeline
* Training and evaluating a regression model

The final output is a **Linear Regression model** evaluated using RMSE.

---

## 📊 Key Insights

Some high-level takeaways from the analysis:

* Median income shows a strong positive relationship with house value
* Location-based features (latitude/longitude, ocean proximity) play a significant role
* Several features are right-skewed, suggesting potential for transformation in future iterations

---

## 📁 Project Structure

```bash
housing-price-prediction/
├── data/
│   └── housing.csv              # Dataset
├── housing_model.ipynb          # Main notebook (EDA + modeling)
├── README.md                    # Project documentation
```

---

## 🧠 Modeling Approach

* **Model:** Linear Regression
* **Preprocessing:**

  * Missing value imputation (median)
  * One-hot encoding for categorical features
* **Pipeline:** `ColumnTransformer` + `Pipeline` (scikit-learn)
* **Train/Test Split:** 80/20

---

## 📈 Evaluation

Model performance is evaluated using:

* **Root Mean Squared Error (RMSE)**

This provides an interpretable measure of average prediction error in housing price units.

---

## 🛠️ Tech Stack

* Python
* pandas, numpy
* matplotlib, seaborn
* scikit-learn

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/pmcelroy4/house_price_model.git
cd housing-price-prediction
```

2. Install dependencies (if applicable):

```bash
pip install -r requirements.txt
```

3. Launch the notebook:

```bash
jupyter notebook housing_model.ipynb
```

---

## 🔮 Future Improvements

* Try more advanced models (Random Forest, Gradient Boosting)
* Add feature engineering (e.g., rooms per household, bedrooms per room)
* Perform cross-validation for more robust evaluation
* Apply scaling or transformations to skewed features

---

## 💡 Why This Project

This project demonstrates:

* A structured approach to EDA and feature understanding
* Practical use of scikit-learn pipelines
* The ability to move from raw data → insights → model

