# Case Study for WQD7005 Data Mining Alternative Assessment 1

## Objective

The case study aims to assess students' ability to apply decision tree and ensemble
methods in a practical context, demonstrating their understanding of the concepts and
their ability to derive meaningful business insights from data analysis.

## Dataset

The dataset used in this case study includes information on customer demographics, purchase history, membership level, and churn status. It can be accessed [here](ecommerce_customer_data_large.csv).

## Methodology

1. I began by cleaning and preparing the dataset. This involved handling missing values, encoding categorical variables, and scaling numerical features to ensure data quality and consistency.
    1. Initial cleaning is done using Python.
    2. More in-depth cleaning through Talend Data Prep.

2. I conducted feature engineering to create relevant attributes from existing data. For example, I derived the "FavoriteCategory" and "LastPurchaseDate" columns from "Product Category" and "Purchase Date."
   1. Derivation of new column is done in Python.
   2. Values derived in new column is made sure to be consistent among the same customer using customer ID as reference.

3. I explored several machine learning models, including Gradient Boosting, Decision Trees, and Random Forest, to predict customer churn. I evaluated model performance using metrics like misclassification rate and squared error.

4. Throughout the analysis, I tackled challenges such as data imbalance and model overfitting. Resampling techniques and hyperparameter tuning were employed to mitigate these issues.

5. While Gradient Boosting excelled in predictive power, Decision Trees were considered for their interpretability. I evaluated the trade-offs between complexity and transparency.

6. I emphasized the importance of ongoing model monitoring and evaluation to adapt to changing customer behavior patterns and maintain predictive effectiveness over time.

## Findings

- Best Model: Gradient Boosting performed the best among the models, showing the lowest misclassification rate on both training and validation data.
- Important Factors: Membership level, purchase history, and payment methods were identified as significant factors affecting customer churn.
- Interpretability: While Gradient Boosting excelled in predictive power, Decision Tree models offered better interpretability.

## Conclusion

In this customer churn study, Gradient Boosting emerged as the top-performing model, offering the lowest misclassification rates on both training and validation data. This model should be the choice for precise churn prediction. I identified vital factors affecting churn, like membership level, and payment methods. These insights guide tailored retention strategies for businesses. We overcame challenges such as data imbalance and model overfitting, underscoring the importance of robust model evaluation.

## Reflections or Learning Outcomes

- This case study has reinforced the importance of thorough model evaluation and selection. 
- Addressing challenges such as data imbalance and overfitting requires creative solutions like resampling and hyperparameter tuning. These experiences have underscored the significance of a flexible and adaptive approach in data science.
- the iterative nature of model deployment and monitoring is crucial for maintaining model effectiveness over time

## Usage

To use the code and replicate the analysis, download and run the Python script in your machine. Change any relevant directory to input and output paths. You can access the [Python script](data_derivation.py) for data preprocessing.

## Contributing

Contributions are welcome! If you have suggestions, improvements, or bug fixes, please open an issue or submit a pull request.
