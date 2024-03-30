**Insurance Prediction Model Documentation**

**Introduction**

This document provides documentation for the Insurance Prediction Model project. The project aims to develop a machine learning model to predict insurance responses based on various features provided in the dataset.

**Installation**

To run the code in this repository, you'll need Python 3.x along with the following dependencies:

matplotlib
pandas
numpy
xgboost
scipy
scikit-learn
tqdm
shap
You can install these dependencies using pip:

bash
Copy code
pip install -r requirements.txt
Usage

Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/insurance-prediction.git
Navigate to the project directory:

bash
Copy code
cd insurance-prediction
Ensure you have the dataset file named train.csv in the project directory.

Run the main script:

bash
Copy code
python insurance_prediction.py
File Structure

insurance_prediction.py: Main script containing the code for data preprocessing, model training, evaluation, and feature selection.
requirements.txt: List of Python dependencies required to run the code.
README.md: Documentation file providing information about the project.
Data

**The dataset** (train.csv) contains information about insurance applicants along with their responses.

**Model Training and Evaluation
**
The XGBoost algorithm is used for model training. Model performance is evaluated using a custom quadratic weighted kappa metric. Feature selection is performed using PCA, and SHAP values are calculated for interpretability.


**Goal**

Our goal was to develop an algorithm for Prudential Life Insurance that optimizes risk assessment processes by reducing the reliance on extensive customer data. We aimed to address customer concerns regarding privacy and data collection while maintaining the accuracy of risk assessment. Through dimensionality reduction techniques, including PCA, t-SNE, and autoencoders, we sought to streamline the decision-making process and enhance the efficiency of insurance operations.

**Our Experimentation and Results
**

We experimented with various feature reduction techniques, starting with a review of existing research and exploring methods such as PCA, t-SNE, and autoencoders. Our experimentation involved preprocessing the Prudential dataset, handling missing values, and feature engineering. We evaluated the performance of different models, including Logistic Regression, Random Forest, and XGBoost, to assess the impact of feature reduction on model accuracy. Our results demonstrated that our approach significantly reduced the dataset dimensions while maintaining a robust performance, with XGBoost achieving a kappa score of 0.65. By balancing model performance with feature selection, we provided valuable insights into enhancing risk assessment processes in the insurance sector.
