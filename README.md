# Global Housing Market Analysis

A comprehensive machine learning project that analyzes global housing markets using XGBoost regression and SHAP explainability techniques.

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## About the Project

This project provides a data-driven approach to understanding global housing market dynamics through machine learning. Using a dataset spanning multiple countries and years, it builds predictive models to forecast house price indices based on various economic and demographic factors.

The analysis includes comprehensive exploratory data analysis, feature engineering, model training with XGBoost, and model interpretability using SHAP values. This makes it valuable for researchers, policymakers, and real estate professionals who need to understand housing market trends and drivers.

## Features

- **Comprehensive Dataset**: 200 entries covering multiple countries from 2015-2023
- **Feature Engineering**: Creates derived features like price-to-rent ratios and real mortgage rates
- **XGBoost Regression**: Advanced gradient boosting for accurate price predictions
- **Model Interpretability**: SHAP analysis for understanding feature contributions
- **Performance Metrics**: RMSE, MAE, MAPE, R², and explained variance scores
- **Visualization**: Actual vs predicted plots and feature importance charts
- **Robust Preprocessing**: Handles infinite values and missing data

## Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook
- Required packages (see installation below)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/GlobalHousingMarketAnalysis.git
cd GlobalHousingMarketAnalysis
```

2. Install required packages:
```bash
pip install pandas numpy xgboost scikit-learn matplotlib seaborn shap
```

3. Launch Jupyter Notebook:
```bash
jupyter notebook
```

4. Open `MachineLearningTutorial.ipynb` and run all cells

### Usage

The notebook is structured to run sequentially:

1. **Data Loading**: Imports the housing market dataset
2. **Exploratory Analysis**: Basic statistics and data overview
3. **Data Preparation**: Feature engineering and train-test split
4. **Model Training**: XGBoost regression with hyperparameter tuning
5. **Evaluation**: Comprehensive performance metrics
6. **Interpretation**: SHAP analysis for model explainability

Simply execute each cell in order to reproduce the analysis.

## Configuration

The model uses the following default parameters:

```python
params = {
    'objective': 'reg:squarederror',
    'learning_rate': 0.01,
    'max_depth': 3,
    'subsample': 0.8,
    'colsample_bytree': 0.7,
    'eval_metric': 'rmse',
    'seed': 42,
    'reg_alpha': 1,
    'reg_lambda': 1
}
```

You can modify these parameters in the notebook to experiment with different model configurations.

## Roadmap

- [ ] Add support for additional countries and time periods
- [ ] Implement time series forecasting capabilities
- [ ] Add interactive visualizations with Plotly
- [ ] Create a web application for real-time predictions
- [ ] Integrate external data sources for automatic updates
- [ ] Add support for different property types (residential, commercial)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Atharva Soundankar](https://www.kaggle.com/atharvasoundankar) for the [Global Housing Market Analysis (2015-2024) dataset](https://www.kaggle.com/datasets/atharvasoundankar/global-housing-market-analysis-2015-2024/data)
- XGBoost team for the excellent gradient boosting framework
- SHAP library for model interpretability tools
- Scikit-learn for machine learning utilities
