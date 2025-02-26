# 🚢Titanic Survival Prediction

This project analyzes the Titanic dataset and predicts passenger survival using Logistic Regression. It includes data preprocessing, model training, evaluation, and visualization.

## 📌 Project Overview

The Titanic dataset contains information about passengers, such as age, gender, ticket class, and whether they survived the disaster. This project aims to build a machine learning model to predict survival based on these features.

## 📊 Dataset Overview

The dataset includes the following key columns:

- `pclass` (Passenger Class): 1st, 2nd, or 3rd class.
- `sex`: Male or Female.
- `age`: Age of the passenger.
- `sibsp`: Number of siblings/spouses aboard.
- `parch`: Number of parents/children aboard.
- `fare`: Ticket fare paid.
- `embark_town`: The port where the passenger boarded.
- `survived` (Target Variable): 1 = Survived, 0 = Did not survive.

## 🔧 Installation & Setup

Make sure you have Python installed, then install the required dependencies:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

## 🚀 Running the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/Atharv564/titanic-survival-prediction.git
   cd titanic-survival-prediction
   ```

2. Run the Python script:

    ```bash
    python main.ipynb
    ```

## ⚙️ Data Preprocessing

### Handling Missing Values:
- `age`: Missing values are filled with the median age.
- `embark_town`: Missing values are filled with the most frequent category.
- `deck`: Dropped due to too many missing values.

### Feature Encoding:
- `sex`, `embark_town`, `who`, and `embarked` are encoded using `LabelEncoder`.

### Feature Scaling:
- `StandardScaler` is used to normalize numerical features.

## 🏆 Model Training & Evaluation

- **Model Used:** Logistic Regression
- **Train-Test Split:** 80% training, 20% testing
- **Evaluation Metrics:**
  - Accuracy Score
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)

## 📊 Results & Insights

- Women had a **higher survival rate** than men.
- Younger passengers had **better survival chances**.
- **Higher-class** passengers were more likely to survive.
- Logistic Regression predicts survival with **moderate accuracy**.

## 📈 Data Visualization

The project includes the following visualizations:

1. **Survival Count by Gender**  
   - A countplot showing survival distribution among males and females.
2. **Age Distribution**  
   - A histogram displaying the distribution of passenger ages.
3. **Correlation Heatmap**  
   - A heatmap to visualize feature correlations.
  
## 👨‍💻 Developed By [Atharv](https://github.com/Atharv564)  
