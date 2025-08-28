
# Titanic Dataset - Data Processing & EDA

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-2.2.3-red.svg)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-green.svg)

## 📖 Overview

This project performs comprehensive data processing and exploratory data analysis (EDA) on the famous Titanic dataset from Kaggle. The goal is to clean the data, handle missing values, encode categorical variables, and visualize key patterns related to passenger survival.

## 📊 Dataset

The dataset used is `train.csv` from the [Kaggle Titanic competition](https://www.kaggle.com/c/titanic). It contains information about passengers aboard the Titanic, including whether they survived or not.

**Original Features:**
- `PassengerId`: Unique ID for each passenger
- `Survived`: Survival (0 = No, 1 = Yes)
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: Passenger's name
- `Sex`: Passenger's sex
- `Age`: Passenger's age
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Ticket`: Ticket number
- `Fare`: Passenger fare
- `Cabin`: Cabin number
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## 🛠️ Data Processing Steps

1.  **Import Libraries**: Used `pandas`, `numpy`, `matplotlib`, and `seaborn`.
2.  **Load Data**: Read the `train.csv` file into a DataFrame.
3.  **Initial Inspection**: Used `df.info()`, `df.describe()`, and `df.nunique()` to understand the data structure, missing values, and unique counts.
4.  **Data Cleaning**:
    - Dropped irrelevant columns: `PassengerId`, `Name`, `Ticket`, `Cabin`.
    - Removed duplicate rows.
5.  **Handling Missing Values**:
    - **Age**: Filled missing values using a sophisticated method based on data quartiles (`mean`, `median`, `mode`).
    - **Embarked**: Filled the two missing values with the most frequent value (`mode`).
6.  **Feature Encoding**:
    - Encoded the `Sex` column: `male` -> `1`, `female` -> `0`.

## 📈 Exploratory Data Analysis (EDA)

Visualizations were created to uncover insights from the cleaned data:

-   **Survival Count**: A countplot showing the overall number of survivors vs. non-survivors.
-   **Survival by Gender**: A countplot showing the relationship between gender (`Sex`) and survival.
-   **Age Distribution**: A histogram showing the distribution of passenger ages.

## 🚀 How to Run the Code

1.  Ensure you have the required libraries installed:
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
2.  Download the `train.csv` file from the [Kaggle Titanic competition page](https://www.kaggle.com/c/titanic/data) and place it in the correct path referenced in the notebook (e.g., `/kaggle/input/titanic/train.csv`).
3.  Open the Jupyter Notebook (`data-processing-for-titanic.ipynb`) and run all cells.

## 🔮 Key Insights

-   The overall survival rate was **38.4%**.
-   There is a very strong relationship between **gender and survival**. A significantly higher proportion of females survived compared to males.
-   The age distribution of passengers is right-skewed, with most passengers being between 20 and 40 years old.


## 👨‍💻 Author

[Abdalla Ehab Hassan]
- Connect with me on [LinkedIn](https://www.linkedin.com/in/yourprofile/)
- Check out my other projects on [GitHub](https://github.com/yourusername)

## 📝 License

This project is for educational purposes. The dataset is provided by Kaggle.
