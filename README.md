# Customer Response Prediction

## Overview
This project predicts whether a customer will accept a marketing offer using machine learning classification models. The workflow includes exploratory data analysis (EDA), feature selection, preprocessing pipelines, model tuning, and ensemble evaluation to identify the most effective predictive approach.

The goal is to help businesses improve marketing efficiency by targeting customers who are more likely to respond positively to promotional campaigns.

---

## Business Problem
Marketing campaigns often result in wasted resources when offers are sent to uninterested customers. Accurately predicting customer response allows organizations to:

- Improve conversion rates
- Reduce marketing costs
- Personalize customer outreach
- Support data-driven marketing decisions

This project builds predictive models to classify whether a customer is likely to accept an offer based on demographic and behavioral features.

---

## Dataset
The dataset contains customer demographic and engagement-related features used to predict the binary target variable:

- `accepted_offer`
  - `1` = customer accepted the offer
  - `0` = customer declined the offer

### Data Characteristics
- Mixed numerical and categorical features
- Class imbalance evaluation performed
- Missing values handled through preprocessing pipelines

---

## Exploratory Data Analysis (EDA)

Key analysis steps included:

- Evaluating missing values
- Identifying class imbalance
- Detecting high-impact categorical variables
- Comparing numerical feature distributions between accepted vs declined offers

### Insights
- Several categorical features showed strong differences in acceptance rates
- Certain numerical features demonstrated meaningful separation between responders and non-responders
- Feature distributions guided feature selection and model preparation decisions

---

## Feature Engineering & Preprocessing

### Preprocessing Pipeline
- Missing value imputation
- One-hot encoding for categorical variables
- Power transformation for numerical features

### Feature Selection
Features with stronger relationships to offer acceptance were prioritized based on:
- acceptance rate spread
- group size thresholds
- median and mean differences between classes

---

## Machine Learning Models

The project evaluates multiple classification models, including:

- Logistic Regression
- Random Forest Classifier
- LightGBM Classifier

### Validation Strategy
- Stratified cross-validation
- Model tuning beyond default parameters
- Ensemble evaluation

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

---

## Results & Findings

### Key Findings
- Tree-based models demonstrated stronger predictive performance than baseline linear models
- Feature selection improved model interpretability while maintaining performance
- Ensemble methods were evaluated to determine whether combining models improved generalization

### Business Impact
The final model can support:
- targeted marketing campaigns
- customer segmentation
- conversion optimization
- efficient allocation of marketing resources

---

## Technologies Used

- Python
- pandas
- NumPy
- scikit-learn
- LightGBM
- matplotlib
- seaborn
- Sweetviz
- Jupyter Notebook

---

## Project Structure

```text
customer-response-prediction/
│
├── notebooks/
├── data/
├── visualizations/
├── README.md
└── requirements.txt
```

---

## How to Run

1. Clone the repository
2. Install required dependencies
3. Open the notebook in Jupyter Notebook or Google Colab
4. Run all cells sequentially

```bash
pip install -r requirements.txt
```

---

## Future Improvements

- Hyperparameter optimization
- Additional ensemble techniques
- Feature importance visualization
- Model deployment as an API or dashboard
- Customer segmentation integration

---

## Author

**Pranika Chandra**  
Data Science & Machine Learning Projects focused on predictive modeling, analytics, and applied AI.
