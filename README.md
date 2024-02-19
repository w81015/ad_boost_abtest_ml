[中文版 Chinese version](README_zh.md)

# Ad Effectiveness Enhancement Program: A/B Testing and Machine Learning Implementation

## Project Overview
This project analyzes the impact of different advertising strategies on user conversion rates through A/B testing and machine learning models, aiming to provide businesses with data-driven advertising optimization strategies.

## Project Structure
- `Exploratory Data Analysis`: Using Pandas for raw data processing and analysis, and NumPy for data calculations, to identify factors affecting conversion rates.
- `A/B Testing`: Evaluating the effectiveness of advertising strategies through the design and implementation of A/B tests, and using statistical methods to verify the significance of the results.
- `Model Building and Evaluation`: Building a random forest prediction model with Scikit-learn and addressing the issue of sample imbalance with the SMOTE technique, enhancing the model's prediction capability for minority classes.
- `Model Application`: Applying the trained model to new datasets for real-time prediction to guide future advertising strategy adjustments.

## Technologies and Tools
- `Pandas` and `NumPy`: For data processing and analysis.
- `Matplotlib` and `Seaborn`: For data visualization, helping to identify data distributions and key trends.
- `Scikit-learn`: For the implementation of machine learning algorithms and model evaluation.
- `SMOTE`: To address the issue of data imbalance, enhancing the learning ability of the model for minority classes.

## Model Training:
```python
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier

# Splitting the dataset into training and testing sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.25)

# Model building
model = RandomForestClassifier()
model.fit(X_train, y_train)

# Model evaluation
accuracy = model.score(X_test, y_test)
print(f'Model accuracy: {accuracy}')
```

## Contribution Guide
Contributions to this project are welcome, whether through feedback, error correction, or the addition of new features.

## Contact Information
For any questions or suggestions, please contact us via email at w81015@gmail.com.
