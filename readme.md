# 🥥 Arecanut Price Forecasting

A machine learning project for predicting arecanut (betel nut) prices using time series analysis and ensemble methods.

## 📊 Project Overview

This project implements and compares multiple forecasting models to predict arecanut prices in the Indian market. It combines traditional time series methods (ARIMA) with modern machine learning approaches (Random Forest) to provide accurate price predictions.

### Key Features
- **Data Processing**: Comprehensive data cleaning and exploratory data analysis
- **ARIMA Model**: Time series forecasting using AutoRegressive Integrated Moving Average
- **Random Forest**: Ensemble learning approach with lag features
- **Model Comparison**: Detailed evaluation and visualization of both approaches
- **Performance Metrics**: MAE, MSE, RMSE, and MAPE calculations

## 📁 Project Structure

```
areca_nut_price_forecasting/
├── notebook/
│   └── arecanut_arima_model.ipynb       # Main analysis notebook
├── data/
│   └── arecanut_price.xls               # Historical price data
├── source/                              # Source code files
├── readme.md                            # This file
└── requirements.txt                     # Python dependencies
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- Git

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Nadvik-K-M/areca_nut_price_forecasting.git
cd areca_nut_price_forecasting
```

2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

## 📚 Usage

### Running the Analysis

Open the Jupyter notebook:
```bash
jupyter notebook notebook/arecanut_arima_model.ipynb
```

The notebook includes the following sections:
1. **Data Loading & Preprocessing** - Load and clean arecanut price data
2. **Exploratory Data Analysis** - Visualize trends and distributions
3. **Stationarity Testing** - ADF test for time series properties
4. **ARIMA Modeling** - Train and evaluate ARIMA(5,1,0) model
5. **Random Forest Modeling** - Create lag features and train ensemble model
6. **Model Comparison** - Compare ARIMA vs Random Forest predictions

## 📊 Dataset

**Source**: Indian market arecanut prices

**Columns**:
- `Variety`: Type of arecanut variety
- `Min Price (Rs./Quintal)`: Minimum daily price
- `Max Price (Rs./Quintal)`: Maximum daily price
- `Modal Price (Rs./Quintal)`: Most frequent price
- `Price Date`: Date of price recording

**Records**: 47,670 historical price entries

## 🤖 Models

### ARIMA Model
- **Order**: (5, 1, 0)
- **Purpose**: Capture temporal dependencies in price data
- **Advantages**: Theoretically sound for time series, interpretable parameters

### Random Forest Model
- **Features**: Lag1, Lag2 (previous day prices)
- **Estimators**: 100 trees
- **Purpose**: Non-linear pattern recognition
- **Advantages**: Handles complex relationships, feature importance insights

## 📈 Results

The notebook generates performance metrics for both models:

```
Performance Metrics:
├── MAE (Mean Absolute Error)
├── MSE (Mean Squared Error)
├── RMSE (Root Mean Squared Error)
└── MAPE (Mean Absolute Percentage Error)
```

Visualizations include:
- Historical price trends
- Price distributions
- Rolling mean and standard deviation
- ARIMA forecast vs actual
- Model comparison plot

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computations |
| **Matplotlib/Seaborn** | Data visualization |
| **Statsmodels** | ARIMA modeling |
| **Scikit-learn** | Machine learning models |

## 📝 Future Enhancements

- [ ] Implement SARIMA for seasonal patterns
- [ ] Add exogenous variables (weather, market conditions)
- [ ] Deploy as REST API
- [ ] Create interactive dashboard
- [ ] Ensemble voting system combining both models
- [ ] Hyperparameter optimization

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

## 📄 License

This project is open source and available under the MIT License.

## 👤 Author

**Nadvik K M**  
GitHub: [@Nadvik-K-M](https://github.com/Nadvik-K-M)

## 📧 Contact & Support

For questions or support, please open an issue on the GitHub repository.

---

**Last Updated**: December 26, 2025  
**Status**: Active Development
