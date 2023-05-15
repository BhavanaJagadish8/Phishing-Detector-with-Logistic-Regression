# Phishing-Detector-with-Logistic-Regression



The provided code performs the following tasks for building and evaluating a phishing website classifier using Logistic Regression:

1. Importing Required Libraries:
   - pandas: Library for data manipulation and analysis.
   - numpy: Library for mathematical operations.
   - matplotlib: Library for data visualization.
   - seaborn: Library for statistical data visualization.
   - sklearn: Library for machine learning algorithms and evaluation metrics.

2. Loading and Preparing the Dataset:
   - The code loads the dataset from the 'phishing.txt' file using pandas' `read_csv` function.
   - The shape of the dataset (number of rows and columns) is printed.
   - Column names are assigned to the dataset.

3. Exploratory Data Analysis:
   - The first five rows of the dataset are displayed using the `head()` function.

4. Building and Evaluating the Classifier:
   - Features and target variables are separated from the dataset.
   - The dataset is split into training and test sets using the `train_test_split` function.
   - A logistic regression classifier is created with a regularization parameter (C) set to 100.
   - The classifier is fitted to the training data.
   - Predictions are made on the test data.
   - The accuracy score of the classifier is calculated using the `accuracy_score` function.
   - The number of misclassified samples is calculated by comparing the predicted labels with the true labels.

5. Selecting Relevant Features:
   - Only the 'PrefixSuffix-' and 'AnchorURL' columns are selected as features.
   - The dataset is split into training and test sets again.
   - Another logistic regression classifier is created and fitted to the training data.
   - Predictions are made on the test data, and the accuracy score is calculated.

6. Plotting the Decision Boundary:
   - A function called `plot_decision_boundary` is defined to visualize the decision boundary of the classifier.
   - The function takes the trained classifier, feature matrix (X), and target variable (y) as inputs.
   - It generates a meshgrid of points covering the feature space and predicts the labels for each point.
   - The decision boundary and test data points are plotted using matplotlib.
   - The plot displays the 'Prefix-Suffix' feature on the x-axis, 'AnchorURL' feature on the y-axis, and class labels as colors.

The code demonstrates the process of building a logistic regression classifier for phishing website classification. It includes data loading, preprocessing, feature selection, model training, prediction, evaluation, and visualization of the decision boundary.
