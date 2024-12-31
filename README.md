## Job Postings Detection Model
This project focuses on detecting fraudulent job postings using machine learning techniques. It involves data preprocessing, feature extraction, and model training using two classifiers: Random Forest and XGBoost. Below is an overview of the workflow, implementation details, and results.

## Project Overview
Fraudulent job postings can cause significant harm to job seekers. This project aims to classify job postings as either fraudulent or legitimate using natural language processing and machine learning techniques.

## Dataset
The dataset used in this project is fake_job_postings.csv. It contains the following key columns:
•	Text Features: company_profile, description, requirements, benefits
•	Numerical Features: telecommuting, has_company_logo, has_questions
•	Target: fraudulent

## Workflow
1.	Data Loading and Exploration
o	Loaded the dataset and displayed basic statistics.
o	Handled missing values by filling text fields with empty strings and dropping rows with missing target values.
2.	Feature Engineering
o	Combined text columns into a single feature combined_text.
o	Applied TF-IDF Vectorization to extract textual features.
o	Combined numerical and text features for model training.
3.	Model Training
o	Split the dataset into training and testing sets (80/20).
o	Trained two models:
	Random Forest Classifier
	XGBoost Classifier
4.	Evaluation Metrics
o	Accuracy
o	ROC-AUC Score
o	Confusion Matrix
o	Classification Report
5.	Feature Importance Analysis
o	Used SHAP for interpretability.
o	Employed permutation importance for Random Forest.

## Results
Model Performance
Metric	Random Forest	XGBoost
Accuracy	90.00%	91.50%
ROC-AUC Score	0.92	0.94
Insights
•	Random Forest: Reliable baseline model with balanced recall and precision.
•	XGBoost: Higher accuracy and ROC-AUC, excels in handling structured data.

## Key Plots
1.	ROC Curve Comparison: Shows the performance of Random Forest and XGBoost.
2.	SHAP Summary Plot: Highlights feature contributions to predictions.
3.	Permutation Feature Importance: Identifies critical features impacting Random Forest predictions.

## Instructions for Use
1.	Dependencies
o	Python 3.x
o	Required Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, shap
2.	Run the Code
o	Load the dataset: Ensure the file fake_job_postings.csv is in the working directory.
o	Execute the script in a Jupyter Notebook or Python environment.
3.	Optimization Notes
o	Reduced dataset size for permutation importance to improve runtime.
o	Adjusted SHAP analysis to handle dense matrix input.

## Future Work
•	Hyperparameter tuning for XGBoost to further improve performance.
•	Exploration of additional models like LightGBM or neural networks.
•	Incorporation of additional features (e.g., metadata).

## Acknowledgments
This project uses the fake_job_postings.csv dataset to address a critical problem in job markets. Special thanks to contributors and developers of Python libraries and tools used in this project.

## Contact
For questions or feedback, please contact Shubham Mohod at mohods193@gmail.com.

