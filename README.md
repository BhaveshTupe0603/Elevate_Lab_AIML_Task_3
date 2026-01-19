# Task 3: Exploratory Data Analysis (EDA) - Elevate Lab AIML Internship

## 📌 Project Overview
This project involves performing Exploratory Data Analysis (EDA) on the classic **Iris Dataset** as part of the Elevate Lab AIML Internship. The primary objective is to understand the underlying structure of the data, visualize feature distributions, detect outliers, and analyze the relationships between different features (Sepal Length, Sepal Width, Petal Length, Petal Width) to determine their importance in predicting the species of the iris flower.

## 🛠 Tools & Technologies
The analysis is implemented using the following technologies:

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)

* **Python:** Core programming language.
* **Pandas:** Used for data manipulation and dataframe management.
* **Matplotlib & Seaborn:** Used for data visualization (Histograms, Box Plots, Heatmaps).

## 📊 Dataset
**Dataset Used:** Iris Dataset

The dataset consists of 150 samples from three species of Iris (*Iris setosa*, *Iris virginica*, and *Iris versicolor*). Four features were measured from each sample:
1.  Sepal Length (cm)
2.  Sepal Width (cm)
3.  Petal Length (cm)
4.  Petal Width (cm)

## 🔍 Methodology
The exploratory analysis follows a structured approach to uncover patterns and insights:

### 1. Feature Distribution
* **Histograms:** Used to visualize the frequency distribution of numerical features (Sepal/Petal dimensions).
* **Insight:** Helps in understanding the skewness and spread of the data.

### 2. Categorical Analysis
* **Count Plots:** Used to verify the balance of the dataset across the three target classes (Species).
* **Insight:** Confirms if the dataset is balanced or if stratifying is needed.

### 3. Outlier Detection
* **Box Plots:** Applied to all numerical features to identify anomalous data points.
* **Insight:** Visualizes the Interquartile Range (IQR) and highlights potential outliers that may affect model performance.

### 4. Correlation Analysis
* **Heatmap:** A correlation matrix visualized as a heatmap to quantify linear relationships between variables.
* **Insight:** Identifies highly correlated features (multicollinearity) and features strongly associated with the target variable.

## 💡 Key Insights & Findings
* **Species Separation:** Petal Length and Petal Width provide the clearest distinction between the three species. *Iris setosa* is linearly separable from the other two based on petal dimensions alone.
* **Correlation:** There is a very strong positive correlation between Petal Length and Petal Width. Sepal Length also shows a positive correlation with Petal dimensions.
* **Outliers:** Minor outliers were detected in the Sepal Width feature, specifically for the *Iris virginica* species.
* **Feature Importance:** Petal features are significantly more important for prediction than Sepal features.

## 🚀 Conclusion
The EDA confirms that the Iris dataset is well-structured and balanced. The strong correlation between petal features suggests that a simple classification model (like Decision Trees or KNN) would likely achieve high accuracy. The clear separation of *Iris setosa* makes it easily identifiable compared to *Versicolor* and *Virginica*, which have some overlap.
