# Titanic Dataset Visualization Project

## Project Overview
This project focuses on analyzing the Titanic dataset to extract meaningful insights and present them using compelling visualizations. The analysis explores passenger demographics, survival rates, and other influential factors that determined survival.

## Dataset
The dataset is sourced from the [Kaggle Titanic dataset](https://www.kaggle.com/c/titanic/data), containing information about passengers, such as:

- **PassengerId**: Unique identifier for each passenger
- **Survived**: Survival status (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1st, 2nd, 3rd)
- **Name**: Passenger's name
- **Sex**: Gender
- **Age**: Age in years
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Ticket**: Ticket number
- **Fare**: Ticket fare
- **Cabin**: Cabin number
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Goals
- Understand the demographic composition of passengers.
- Identify the factors influencing survival rates.
- Visualize trends and insights using Python libraries like Matplotlib, Seaborn, and Plotly.

## Tools and Libraries
- **Python**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical operations
- **Matplotlib**: Data visualization
- **Seaborn**: Statistical data visualization
- **Plotly**: Interactive visualizations

## Steps

### 1. Data Loading and Preprocessing
- Load the dataset.
- Handle missing values.
- Convert categorical variables to numeric using encoding techniques.

### 2. Exploratory Data Analysis (EDA)
- Explore the structure of the dataset.
- Generate descriptive statistics.
- Visualize distribution of key features (e.g., Age, Fare).

### 3. Key Questions Explored
- What was the survival rate across different classes and genders?
- Did age or fare have a significant influence on survival?
- How did the port of embarkation affect survival chances?

### 4. Visualizations
#### Example Charts:
- **Bar Chart**: Survival rate by passenger class and gender.
- **Histogram**: Age distribution of survivors vs non-survivors.
- **Heatmap**: Correlation between numerical features.
- **Boxplot**: Fare distribution across different classes.
- **Pie Chart**: Proportion of survivors vs non-survivors.
- **Scatter Plot**: Relationship between age and fare.

### 5. Key Insights
- Survival rates were higher for females and first-class passengers.
- Younger passengers had slightly better survival chances.
- Passengers who paid higher fares were more likely to survive.

## Sample Visualizations
### 1. Survival Rate by Gender
```python
sns.barplot(x='Sex', y='Survived', data=titanic_data)
plt.title('Survival Rate by Gender')
plt.show()
```

### 2. Age Distribution
```python
sns.histplot(titanic_data['Age'], kde=True, bins=30, hue=titanic_data['Survived'])
plt.title('Age Distribution: Survivors vs Non-Survivors')
plt.show()
```

## Conclusion
This project highlights how data visualization can uncover patterns and trends in a dataset. The analysis provides insights into the factors that influenced survival on the Titanic and demonstrates the power of combining statistical methods with visual storytelling.

## Future Work
- Implement machine learning models to predict survival.
- Enhance visualizations with interactive tools like Dash or Tableau.
- Dive deeper into the relationship between ticket prices and survival.

## References
- [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Matplotlib Documentation](https://matplotlib.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
