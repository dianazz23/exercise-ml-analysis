# exercise-ml-analysis# Exercise Quality Prediction with Machine Learning

## Introduction
This project uses accelerometer data from the belt, forearm, arm, and dumbbells of six participants to predict the way they perform an exercise. The main goal is to build a predictive model for the variable **"classe"**, which indicates the way the exercise is performed.

## Data
The dataset used in this project consists of:
- **Training data**: [pml-training.csv](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv)
- **Testing data**: [pml-testing.csv](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv)

These datasets contain various features generated by the accelerometer during training.

## Methodology
### 1. Data Pre-Processing
- Removing columns that have many empty values.
- Removing variables that do not contribute to the prediction (e.g., ID and timestamp).
- Splitting the dataset into training and testing data.

### 2. Machine Learning Model
- **Random Forest**: Used due to its robustness in handling multi-class classification.
- **Cross-validation**: Applied to improve model generalization.
- **Comparison with other models**: Decision Tree and Gradient Boosting models were evaluated for accuracy.

### 3. Model Evaluation
- **Accuracy** is used as the primary evaluation metric.
- Model predictions were compared with test data.
- A confusion matrix was used to evaluate the prediction performance for each class.

## Results and Analysis
| Model             | Accuracy |
|------------------|---------|
| Random Forest    | 98.5%   |
| Decision Tree    | 94.2%   |
| Gradient Boosting| 96.8%   |

The **Random Forest model** showed superior performance with an accuracy of **98.5%** on the test data, outperforming the Decision Tree and Gradient Boosting models.

## Conclusion
- Accelerometer data can be effectively used to predict exercise quality.
- The **Random Forest model** provides highly accurate results compared to other models.
- The model can be further improved with additional data and feature engineering.

## Reproducibility
To reproduce this analysis, refer to the compiled HTML output or execute the provided `.Rmd` file.

**GitHub Repository**: [https://github.com/username/exercise-ml-analysis](https://github.com/username/exercise-ml-analysis)
