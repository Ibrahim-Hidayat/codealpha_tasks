# Iris Flower Classification

Classifies Iris flowers (setosa, versicolor, virginica) from four measurements.
Built for the CodeAlpha Data Science Internship (Task 1).

## Dataset
150 flowers, 4 features (sepal and petal length/width in cm), 3 balanced
classes (50 each), no missing values. File: `Iris.csv`.

## Approach
1. Loaded and explored the data with pandas
2. Visualized feature relationships with a seaborn pairplot
3. Split into 80% training / 20% testing (stratified)
4. Trained a K-Nearest Neighbors classifier (k=5)
5. Evaluated with accuracy, classification report and confusion matrix
6. Compared 4 models using 5-fold cross-validation

## Results
- KNN accuracy on the held-out test set (30 flowers): 100%
- 5-fold cross-validation accuracy:

| Model | Mean accuracy |
|---|---|
| KNN | 0.973 |
| Logistic Regression | 0.973 |
| SVM | 0.967 |
| Decision Tree | 0.953 |

## Key findings
- Setosa is clearly separable from the other two species.
- Versicolor and virginica overlap slightly, mostly in sepal measurements.
- Petal measurements are the most informative features.
- All four models perform similarly (about 95-97%).

## Tools
Python, pandas, scikit-learn, seaborn, matplotlib, Google Colab
