# Fake Job Posting Prediction Model

This repository contains a machine learning project focused on detecting fake job postings using data analysis and predictive modeling. The repository includes a Jupyter Notebook, dataset, and a detailed project report.

## Contents

- **Project_Model_Final.ipynb**: The main notebook containing all the code, explanations, and visualizations for the project.
- **report fake job.pdf**: A detailed project report summarizing objectives, methodologies, results, and conclusions.
- **Companies_Information.csv**: Dataset containing company-related information used as part of the analysis.

## Objective

The objective of this project is to classify job postings as genuine or fraudulent based on features and patterns in the dataset.

## Features

- **Data Preprocessing**:
  - Cleaning, handling missing values, and encoding categorical variables.
  - Text preprocessing with tokenization, stop word removal, and TF-IDF vectorization.
- **Exploratory Data Analysis (EDA)**:
  - Visualization of patterns in genuine vs. fraudulent postings.
  - Insights into textual and numerical data trends.
- **Model Development**:
  - Logistic Regression: Baseline model achieving 91% accuracy.
  - Random Forest Classifier: Improved performance with 97% accuracy.
  - XGBoost: Best-performing model with 98% accuracy, precision of 0.96, and recall of 0.94.
- **Evaluation Metrics**:
  - Accuracy, Precision, Recall, and F1-Score.

## Requirements

To run this project, you'll need the following tools and libraries:

- Python 3.7 or higher
- Jupyter Notebook
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - xgboost

Install the required libraries using:
```bash
pip install -r requirements.txt
```

> **Note**: Ensure to list all the necessary libraries and their versions in the `requirements.txt` file.

## Usage

1. Clone this repository to your local machine:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd <repository-directory>
   ```
3. Place the required dataset (`Companies_Information.csv`) in the appropriate folder.
4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Project_Model_Final.ipynb
   ```
5. Run the cells sequentially to execute the project.

## Results

The project successfully developed a machine learning model to predict fake job postings with high accuracy. Key findings include:

- Fake postings often feature vague job descriptions and missing details.
- XGBoost proved to be the most reliable model with an F1-Score of 0.95.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

For more projects, visit my GitHub profile: [Shubham Mohod](https://github.com/shubhs842).

## Acknowledgments

- Dataset and preprocessing inspiration.
- Libraries and frameworks used in this project.
- Report summarizing project objectives and results.
