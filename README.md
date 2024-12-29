# Heart Stroke Prediction Using Machine Learning

## Project Overview

This project focuses on leveraging advanced machine learning techniques to predict the risk of heart strokes. By analyzing key risk factors such as age, average glucose level, BMI, hypertension, and lifestyle choices, this AI-based solution aims to revolutionize healthcare by enabling early detection, timely intervention, and personalized healthcare strategies.

## Objectives

1. **Predictive Model:** Develop a model to accurately predict individuals at risk of experiencing a heart stroke.
2. **Factor Analysis:** Identify and analyze significant factors contributing to heart stroke risk, such as medical history, lifestyle choices, and physical activity levels.

## Dataset

The dataset used in this project is sourced from Kaggle: [Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset/data).

### Dataset Description

The dataset includes attributes such as age, gender, BMI, average glucose level, smoking status, and the target variable indicating stroke occurrence.

## Methodology

### Data Preprocessing

- Handling missing values (e.g., filling missing BMI values with the median).
- Encoding categorical variables.
- Scaling numerical features.
- Addressing class imbalance using the Synthetic Minority Over-sampling Technique (SMOTE).

### Models Implemented

1. **Logistic Regression**:
   - Achieved accuracy: 84%.
   - Utilized SMOTE for class balancing.

2. **Support Vector Machines (SVM)**:
   - Achieved accuracy: 84%.
   - Utilized kernel functions such as linear, RBF, and polynomial.

3. **Decision Trees**:
   - Achieved accuracy: 89%.
   - Tuned parameters for better performance.

4. **Random Forest**:
   - Achieved accuracy: 92%.
   - Chosen as the best model due to high precision and accuracy.

5. **XGBoost**:
   - Achieved accuracy: 92%.

6. **CatBoost**:
   - Achieved accuracy: 92%.

### Evaluation Metrics

- Accuracy, Precision, Recall, and F1 Score were used for evaluation.
- Confusion matrix analysis provided insights into the model's performance for both stroke and non-stroke predictions.

## Key Findings

- **Top Contributing Factors**:
  - Age
  - Average Glucose Level
  - BMI
  - Work Type
  - Smoking Status

- **Best Performing Model**:
  - Random Forest was selected due to its high accuracy (92%) and precision for stroke predictions.

## Results and Impact

1. **Improved Predictive Accuracy**: The models achieved high accuracy in identifying individuals at risk of heart strokes.
2. **Healthcare Applications**: Findings can inform proactive healthcare interventions, saving lives and reducing costs.
3. **Personalized Interventions**: Enables tailored healthcare strategies based on individual risk profiles.

## Installation and Usage

```bash
# Clone the repository
git clone https://github.com/yourusername/heart-stroke-prediction.git

# Install the required dependencies
pip install -r requirements.txt

# Run the preprocessing and training scripts
python train_model.py

# Use the prediction script to test the model on new data
python predict.py --input test_data.csv
