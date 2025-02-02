# CropPricePrediction

This repository contains an end-to-end machine learning project designed to predict the prices of agri-horticultural commodities, including pulses and vegetables. The model leverages **XGBoost**, **Random Forest**, and **LightGBM** algorithms to provide robust and accurate price predictions.

## Overview

Agricultural price prediction is vital for ensuring fair trade, avoiding market imbalances, and helping farmers make informed decisions. This project explores different machine learning techniques to predict crop prices using historical and categorical data.

---

## Features

- **Machine Learning Algorithms**: Implements and compares the performance of XGBoost, Random Forest, and LightGBM.
- **Scalable Design**: The code is modular, allowing the easy addition of new algorithms or feature transformations.
- **Data Visualization**: Includes plots to analyze feature importance and residuals.

---

## Dependencies

Ensure you have the following Python packages installed:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`
- `lightgbm`
- `jupyter`

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---

## Data

The dataset includes historical prices and relevant features such as:

- **Commodity type**: e.g., vegetables, pulses.
- **Geographical location**: region/state where the data is collected.
- **Temporal information**: time-based features like month and year.
- **Weather data (optional)**: climatic conditions affecting yield and price.

Preprocessing steps include:

1. Handling missing data.
2. Encoding categorical features.
3. Feature scaling for model-specific requirements.

---

## Model Training

The following models are trained and evaluated:

1. **XGBoost**: Known for its gradient-boosting efficiency and feature importance insights.
2. **Random Forest**: Offers interpretability and is robust against overfitting for tabular data.
3. **LightGBM**: Provides faster computation and reduced memory usage for large datasets.

Training involves:

- Splitting the data into train and test sets.
- Performing hyperparameter tuning using GridSearchCV/RandomizedSearchCV.
- Evaluating models using metrics like RMSE, MAE, and R².

---

## Evaluation

- **Metrics Used**: RMSE, MAE, R².
- **Feature Importance**: Visualized to interpret the contributions of individual features.
- **Cross-Validation**: Applied to ensure the robustness of the models.

---

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/username/crop-price-prediction.git
   cd crop-price-prediction
   ```

2. Run the Jupyter Notebook for an interactive experience:
   ```bash
   jupyter notebook Crop.ipynb
   ```

3. Modify the `config.json` file to adjust parameters like the dataset path or model type.

---

## Results

| Model                     | MSE       | R²     |
|---------------------------|-----------|--------|
| GradientBoosting          | 0.000281  | 0.9844 |
| XGBoost                   | 0.000362  | 0.9799 |
| Random Forest             | 0.000356  | 0.9802 |
| LightGBM                  | 0.000945  | 0.9476 |

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

---

Let me know if you want any sections updated with content from your notebook or any specific visualizations!
