# PRODIGY_DS_03
To build and evaluate a Decision Tree Classifier using the Bank Marketing Dataset, which contains data related to a direct marketing campaign by a Portuguese bank. The goal is to predict whether a client will subscribe to a term deposit (`y` = yes or no).

Steps Performed:
1. Load Dataset
The dataset is loaded using pandas with semicolon (;) as the delimiter.

2. Data Preprocessing
 Categorical variables are encoded using one-hot encoding via `pd.get_dummies`.
 The target variable is `y_yes` (1 if the client subscribed, 0 otherwise).
 The feature set `X` contains all other encoded features.

3. Train-Test Split
 The dataset is split into training (80%) and testing (20%) sets using `train_test_split`.

4. Model Training
 A Decision Tree Classifier is trained with a maximum depth of 4 to limit complexity and reduce overfitting.
 The model is trained using `X_train` and `y_train`.

5. Model Evaluation
 The trained model is used to predict outcomes on the test set.
 Evaluation metrics include:
   Accuracy score
   Classification report (precision, recall, f1-score)

6. Decision Tree Visualization
 The trained decision tree is visualized using `plot_tree()` from `sklearn.tree`.
 Feature names and class names are labeled for better interpretability.

Libraries Used:
pandas, numpy: For data handling and preprocessing
matplotlib.pyplot: For plotting
scikit-learn: For model training, evaluation, and tree visualization

