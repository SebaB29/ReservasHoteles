# 🏨 Hotel Booking Cancellation Predictor

A comprehensive Data Science project focused on predicting hotel reservation cancellations. Developed as a competitive entry for a **Kaggle** challenge, this repository showcases a full machine learning pipeline: from Exploratory Data Analysis (EDA) and data cleaning to advanced ensemble modeling and Neural Networks.



# 📸 Project Overview
The objective was to predict the `is_canceled` target variable using a dataset of ~62,000 reservations with 31 features. The project was structured in checkpoints (CHP) to iterate from simple baselines to complex stacked architectures.

# 📍 Table of Contents
- [📝 Description](#-description)
  - [🔍 Predictive Models](#-predictive-models)
  - [🏗️ Development Stages](#️-development-stages)
- [📊 Performance Report](#-performance-report)
- [📈 Key Insights](#-key-insights)
- [🛠️ Technologies](#️-technologies)
- [👥 Team](#-team)
- [📄 License](#-license)

---

# 📝 Description
This project was developed for **Data Organization (95.58)** at FIUBA. It involves handling real-world data issues such as missing values, class imbalance, and outliers to improve prediction accuracy on the Kaggle leaderboard.

## 🔍 Predictive Models
To find the best performance, we explored and tuned a variety of algorithms:
- **Classic Classifiers:** Decision Tree, KNN, SVC.
- **Ensemble Learning:** Random Forest, **XGBoost** (Fastest & most efficient).
- **Meta-Models:** VotingClassifier & **StackingClassifier** (Best performance).
- **Deep Learning:** Neural Networks (Multi-layer Perceptron).

## 🏗️ Development Stages
1. **EDA & Preprocessing:** - Statistical exploration using Pandas & Scipy.
   - Data visualization with Seaborn & Matplotlib.
   - Outlier detection and missing value imputation.
2. **Feature Engineering:** Encoding categorical variables and scaling numerical features for model compatibility.
3. **Training & Validation:** Hyperparameter tuning and cross-validation to prevent overfitting.

---

# 📊 Performance Report

The following table summarizes our best results across different iterations:

| Milestone | Best Model            | F1 Score    | Precision   | Recall      | Accuracy    | Kaggle Score |
| :-------- | :-------------------- | :---------- | :---------- | :---------- | :---------- | :----------- |
| **CHP 2** | Decision Tree         | 0.85184     | 0.84518     | 0.83861     | 0.84570     | 0.84082      |
| **CHP 3** | **Stacking (Winner)** | **0.86116** | **0.86498** | 0.86884     | **0.86379** | **0.86193**  |
| **CHP 4** | Neural Network        | 0.82974     | 0.76997     | **0.89957** | 0.81459     | 0.80829      |

---

# 📈 Key Insights
- **The Power of Stacking:** Combining multiple models through a `StackingClassifier` yielded our highest score, proving that model diversity reduces bias and variance.
- **XGBoost Efficiency:** Identified as the best "price-performance" model, offering very high accuracy with significantly lower training time compared to ensembles or networks.
- **Data Quality Matters:** The initial preprocessing (handling outliers and missing data) was more impactful for the final score than choosing the most complex model.

---

# 🛠️ Technologies
- **Language:** Python 3.x
- **Data Analysis:** Pandas, NumPy, Scipy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, XGBoost
- **Platform:** Kaggle, Jupyter Notebooks

---

# 👥 Team
| Member | Github |
| :--- | :--- |
| **Sebastián Brizuela** | [@SebaB29](https://github.com/SebaB29) |
| **Lucia Agha Zadeh Dehdeh** | [@Lucia-azd](https://github.com/Lucia-azd) |
| **Juan Sebastián Del Río** | [@S2JuanS2](https://github.com/S2JuanS2) |

---

# 📄 License
This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
