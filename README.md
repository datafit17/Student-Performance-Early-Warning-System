# Student-Performance-Early-Warning-System
This project develops a Machine Learning-based Early Warning System to proactively identify students at risk of underperforming academically.
Utilizing data on study habits, participation, personal well-being, and socio-contextual factors, the model predicts the likelihood of a student achieving a final exam score below 70 points.

Key Features:
Predictive Modeling: Implements an optimized RandomForestClassifier to identify patterns associated with low academic performance.
Advanced Preprocessing: Handles nominal and ordinal categorical variables, and standardizes numerical data using a robust ColumnTransformer.
Class Balancing: Incorporates SMOTE within the training pipeline to address class imbalance in the target variable ('low performance'), enhancing the model's ability to detect minority cases.
Hyperparameter Optimization: Utilizes RandomizedSearchCV with stratified cross-validation (StratifiedKFold) to find the best model parameters, ensuring robust evaluation and selection.
Comprehensive Evaluation: Model performance is assessed using key metrics such as the classification report (precision, recall, F1-score), Confusion Matrix, ROC curve and AUC-ROC, as well as the Precision-Recall curve and AUC-PR, which are crucial for imbalanced datasets.
Model Interpretation: Analyzes feature importances (feature_importances_) to understand which factors most significantly influence the risk of low performance, providing actionable insights.
Simplified Deployment Flow: Includes functionality to save and load the complete model pipeline (joblib), facilitating its use for new predictions on unseen student data.

Impact:
The proposed system enables educational institutions to intervene early and in a personalized manner, offering targeted support to students who need it most, thereby fostering improved academic performance and overall well-being.
