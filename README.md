# Predictive Modeling with Fuel Cell Performance Data

This repository contains the implementation of predictive modeling on the Fuel_cell_performance dataset. The analysis focuses on dividing the dataset into specific target groups based on roll numbers and evaluating multiple machine learning models.The analysis leverages the PyCaret library for automating machine learning workflows, including feature selection, outlier removal, normalization, and model comparison.

Since the Roll number is 102203820 i.e. ending with 0 so target variable is target1.



****Model Comparison Result before Pre-Processing****

<img width="736" alt="before" src="https://github.com/user-attachments/assets/16e4f991-ce81-47f1-9a08-db92c562c939" />



****Key Preprocessing Techniques****

*Feature Selection: Identified the most relevant features using univariate analysis, reducing dimensionality and improving computational efficiency.

*Outlier Removal: Applied the Local Outlier Factor (LOF) method to filter out anomalies, enhancing data quality.

*Normalization: Standardized feature scales using Z-score normalization to ensure consistency.

*Transformation: Improved data distribution using Yeo-Johnson transformation for better model fitting.

*Principal Component Analysis (PCA): Reduced dimensionality using incremental PCA to capture the most significant variance in the data.



****Combined Preprocessing****

The preprocessing steps were also tested in combination, significantly enhancing model performance by addressing multiple data quality issues simultaneously.



****Model Comparison Result after combined Preprocessing****

<img width="728" alt="after" src="https://github.com/user-attachments/assets/97b22e89-3f2e-401d-b81b-17db4edd20d8" />



****Prediction Models Validation Curves****


*Bayesian Ridge Regression

![br-validation curve](https://github.com/user-attachments/assets/3a84ad37-de59-46d4-a1f6-3601997861f8)


*AdaBoost Regressor:

![ada-vc](https://github.com/user-attachments/assets/3896a712-bc77-4e34-9b03-1ebe8feec182)


*Least Angle Regression (LAR)

![leastaangleregressor-vc](https://github.com/user-attachments/assets/ddff3413-4295-4c59-a7da-6abfef97f0cc)




****Broader Insights****

*Impact of Preprocessing: The integration of preprocessing techniques such as feature selection, normalization, and outlier removal demonstrated a significant improvement in model accuracy and robustness. These steps collectively mitigated challenges posed by noisy and imbalanced data.

*Model Behavior: Bayesian Ridge consistently outperformed other models, indicating its reliability for the given dataset. Meanwhile, models like AdaBoost effectively handled more complex relationships, albeit with higher computational costs. LAR offered an efficient alternative for tasks with simpler requirements.


