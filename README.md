# Task-7-Support-Vector-Machines-SVM-
Use of SVMs for linear and non-linear classification.

 1. Load and Prepare the Dataset
The dataset is loaded from a CSV file (breast-cancer.csv). Non-numeric columns are dropped, and missing values are handled. The feature matrix X and target vector y are extracted. If the target values are continuous, they are converted into binary classes based on the median.

 2. Data Splitting and Preprocessing
The data is split into training and testing sets using train_test_split. Features are standardized using StandardScaler to ensure SVM performs optimally.

 3. Train SVM Models
Two SVM models are trained:

A linear SVM using a linear kernel.

An RBF SVM using the radial basis function kernel.

Both models are trained on the scaled training data.

 4. Visualize Decision Boundaries
Since the original data has many features, PCA (Principal Component Analysis) is used to reduce the features to 2D for visualization. Decision boundaries for both SVM models are plotted in this reduced 2D space.

 5. Hyperparameter Tuning
A GridSearchCV is used to find the best hyperparameters for the RBF SVM. It searches over a grid of C and gamma values using 5-fold cross-validation.

 6. Model Evaluation
The best model found via grid search is evaluated using:

Cross-validation accuracy scores

Test set classification report including precision, recall, and F1-score

This helps measure the model’s performance and generalization.
