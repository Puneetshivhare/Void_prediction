
# Void Prediction using Machine Learning

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Approach](#approach)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Challenges and Improvements](#challenges-and-improvements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
Friction stir welding (FSW) is a widely used technique in the manufacturing industry for joining materials with high strength and durability. However, the presence of voids in FSW can compromise the quality and integrity of the welds. This project aims to develop a machine learning model that can accurately predict the presence of voids in FSW, allowing for early detection and preventive measures.This project involves predicting the occurrence of voids in materials or manufacturing processes using machine learning techniques. The project utilizes **Logistic Regression** and **Decision Tree** classifiers to analyze the data and predict void occurrences based on certain features.

The goal is to achieve high prediction accuracy to help reduce material defects and optimize quality control processes in manufacturing.

**Key Features:**
- Prediction of voids using **Logistic Regression** and **Decision Tree** classifiers.
- Evaluation of model performance using accuracy, precision, recall, and F1-score.
- Comparison of both algorithms to select the better-performing model for void prediction.

## Dataset
The dataset used for this project includes various features that are indicative of void formation, such as:
- Material properties (density, porosity, etc.)
- Environmental conditions (temperature, humidity, etc.)
- Process parameters (pressure, speed, etc.)

You can obtain the dataset from sources like manufacturing process data or publicly available repositories. The data requires preprocessing to handle missing values and outliers.

## Approach
1. **Data Collection & Cleaning**: Collected relevant data, cleaned it by handling missing values, and standardized it for model building.
2. **Feature Engineering**: Performed feature selection and transformation to optimize input variables.
3. **Model Development**:
   - Built a **Logistic Regression** classifier for binary classification.
   - Built a **Decision Tree** classifier to capture more complex relationships in the data.
4. **Model Evaluation**: Evaluated both models using performance metrics such as **accuracy**, **precision**, **recall**, and **F1-score**.
5. **Model Comparison**: Compared the performance of Logistic Regression and Decision Tree to identify the better approach for void prediction.

## Project Structure
```
Void-Prediction-ML/
│
├── data/
│   ├── void_data.csv                   # Dataset for void prediction
│
├── notebooks/
│   ├── data_preprocessing.ipynb         # Data preprocessing and cleaning
│   ├── model_building.ipynb             # Model building and evaluation
│
├── src/
│   ├── data_processing.py               # Data processing functions
│   ├── model_logistic_regression.py     # Logistic Regression model
│   ├── model_decision_tree.py           # Decision Tree model
│   ├── evaluate.py                      # Script for model evaluation
│
├── README.md                            # Project documentation
└── requirements.txt                     # Python package requirements
```

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/Void-Prediction-ML.git
   cd Void-Prediction-ML
   ```

2. **Install Required Packages**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. **Prepare the Dataset**:
   Place the `void_data.csv` file in the `data/` folder.

2. **Run Data Processing**:
   Preprocess the dataset by running:
   ```bash
   python src/data_processing.py
   ```

3. **Train Logistic Regression Model**:
   ```bash
   python src/model_logistic_regression.py
   ```

4. **Train Decision Tree Model**:
   ```bash
   python src/model_decision_tree.py
   ```

5. **Evaluate Models**:
   Evaluate and compare both models by running:
   ```bash
   python src/evaluate.py
   ```

## Results
The **Logistic Regression** model achieved a reasonable accuracy for simple linear relationships in the dataset, whereas the **Decision Tree** model captured more complex patterns in the data.

Performance metrics:
- **Accuracy**: 
  - Logistic Regression: ~XX%
  - Decision Tree: ~YY%
- **Precision**: 
  - Logistic Regression: ~XX%
  - Decision Tree: ~YY%
- **Recall**:
  - Logistic Regression: ~XX%
  - Decision Tree: ~YY%
- **F1-Score**: 
  - Logistic Regression: ~XX%
  - Decision Tree: ~YY%

Based on these metrics, the Decision Tree showed better overall performance in predicting voids, especially with non-linear relationships.

## Challenges and Improvements
- **Challenges**: Balancing the dataset for void prediction was challenging, and tuning hyperparameters for the Decision Tree was computationally intensive.
- **Improvements**:
  - Employ **Grid Search** or **Random Search** to optimize hyperparameters.
  - Explore ensemble methods like **Random Forest** or **Gradient Boosting** to further improve prediction accuracy.
  - Use **cross-validation** for more robust model evaluation.

## Contributing
Feel free to fork this repository, make improvements, and submit a pull request. Any contributions are welcome!

## License
This project is licensed under the **MIT License**.

---

You can adjust the exact performance numbers (XX% and YY%) once you have them from your model evaluations. This README provides a comprehensive guide for users to understand and use your project.
