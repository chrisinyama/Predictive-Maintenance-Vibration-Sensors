## Predictive Maintenance Using Vibration Sensor Readings on Machinery

**Introduction**

Predictive maintenance is paramount in manufacturing to mitigate unplanned downtime and reduce maintenance costs. This project focuses on developing a predictive maintenance system leveraging vibration sensor data from the "FaultDataset.csv." These readings encompass 9292 rows and 21 columns, with the final column denoting machinery faults (0 for none, 1 for detected fault).

Project Objective
The goal is to deploy machine learning models for identifying and categorizing faults in machinery, ultimately enhancing maintenance efficiency and reducing downtime.

**Dataset Description**
The "FaultDataset.csv" contains sensor readings and fault identification, crucial for predictive maintenance. It offers a comprehensive dataset for training and evaluating models in fault detection.

**Methodology**
Exploratory Data Analysis (EDA)
Schema description
Data size assessment
Summary statistics
Target variable distribution visualization
DataFrame content inspection

**Data Cleaning and Preprocessing**

Handling null values
Feature transformation using RFormula
Splitting dataset into training and test 

**Model Training and Evaluation**
Decision Tree Classifier
RandomForest
Logistic Regression
LinearSVC
MLflow experiment tracking
Comparison of Classification Algorithms
Model performance evaluation
Optimal model selection (RandomForest achieved 0.99 accuracy)
Results and Findings
The RandomForest emerged as the most effective model with 0.99 accuracy, exhibiting robust fault detection capability within machinery.

Models Explored
Decision Tree Classifier
RandomForest
Logistic Regression
LinearSVC
Dataset Utilization
The dataset encompasses various machinery-related features alongside fault labels, facilitating model training and evaluation.

**Model Performance/Results**
After training, evaluating, and tuning the models using big data tools, the following results were obtained:

Decision Tree Classifier: Achieved an accuracy of 0.96 with the best hyperparameters, demonstrating the effectiveness of the distributed decision tree algorithm.

Random Forest Classifier: Outperformed other models with an accuracy of 0.99, leveraging the parallel processing capabilities of Spark and the ensemble technique.

Logistic Regression: Achieved an AUC-ROC score of 0.93, indicating the logistic regression model's ability to distinguish between positive and negative classes. The distributed nature of Spark facilitated efficient training and evaluation.

LinearSVC: Achieved an accuracy of 0.807 after hyperparameter tuning, benefiting from the scalable and parallel processing capabilities of Spark's LinearSVC implementation.

**Tools Used**
The project is implemented using:
Python
Apache Spark's MLlib
Databricks
**Installation and Usage**
Clone the repository: git clone https://github.com/your-username/fault-detection.git
Install dependencies: pip install -r requirements.txt
Download the "FaultDataset.csv" and place it in the appropriate directory.
Execute the main script: python main.py

Conclusion
Based on the evaluation, the RandomForest model is the most suitable for fault detection in manufacturing processes due to its high accuracy.
