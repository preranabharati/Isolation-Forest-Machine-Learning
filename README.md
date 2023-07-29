# Isolation-Forest-Machine-Learning
Outlier Detection Using Isolation Forest and LOF

This code demonstrates outlier detection using two different methods: Isolation Forest and Local Outlier Factor (LOF) on the IRIS dataset.


1. Importing the necessary libraries.

2. Loading the Iris dataset and preparing the data. The dataset is loaded using the `load_iris()` function from scikit-learn, and the features are stored in `X`, while the target (class labels) is stored in `y`.

3. Applying Isolation Forest for outlier detection on the Iris dataset. The `IsolationForest` is initialized with hyperparameters `contamination=0.1` (which means that the model expects 10% of the data to be outliers) and `random_state=42` (for reproducibility). The model is then fitted to the data using the `fit_predict` method, and the predictions are stored in `y_pred_iso`.

4. Applying Local Outlier Factor (LOF) for outlier detection on the Iris dataset. The `LocalOutlierFactor` is initialized with the same contamination value as Isolation Forest. The model is fitted to the data using the `fit_predict` method, and the predictions are stored in `y_pred_lof`.

5. Plotting the outliers detected by Isolation Forest. This code creates a scatter plot where the outliers predicted by the Isolation Forest are shown in red and the inliers are shown in blue. The first two features (sepal length and sepal width) of the Iris dataset are used for visualization.

6. Plotting the outliers detected by Local Outlier Factor. This code creates a scatter plot where the outliers predicted by the Local Outlier Factor are shown in red and the inliers are shown in blue. The first two features (sepal length and sepal width) of the Iris dataset are used for visualization.

The purpose of this code is to visually assess how well the Isolation Forest and Local Outlier Factor models can detect outliers in the Iris dataset based on the sepal length and sepal width features. Note that the dataset has four features in total, but only two are used for visualization purposes.
