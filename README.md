# Forecasting Used Car Prices: A Data-Driven Approach

## Overview
This project focuses on predicting the selling prices of used cars using machine learning techniques. By analyzing key car attributes such as age, mileage, engine capacity, and more, the model provides accurate price recommendations, which can be integrated into car trading platforms.

## Dataset
- **Source**: [Car Price Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/sukhmandeepsinghbrar/car-price-prediction-dataset)
- **Fields**:
  - `Name`: Car make and model.
  - `Year`: Manufacturing year of the car.
  - `Selling Price`: Actual selling price of the car (target variable).
  - `Kilometers Driven`: Distance traveled by the car in kilometers.
  - `Fuel`: Type of fuel used by the car (e.g., Petrol, Diesel).
  - `Seller Type`: Individual or dealer.
  - `Transmission`: Manual or automatic.
  - `Owner`: Number of previous owners.
  - `Mileage`: Fuel efficiency in km/l.
  - `Engine`: Engine capacity in CC.
  - `Max Power`: Maximum power output in BHP.
  - `Seats`: Number of seats.

## Objectives
1. Develop a model to predict used car selling prices based on various features.
2. Perform feature engineering and exploratory data analysis (EDA) to understand the dataset.
3. Evaluate the model using appropriate metrics (MAE, MSE, RMSE).
4. Provide predictions for new test data.

## Workflow

### 1. **Data Preprocessing**
- Addressed missing values and outliers.
- Consolidated infrequent car names under a general "Other" category.
- Created new features like car age.
- Scaled and encoded categorical features.

### 2. **Exploratory Data Analysis (EDA)**
- Analyzed distributions of key features and the target variable.
- Created visualizations such as heatmaps to study correlations.

### 3. **Model Development**
- **Algorithm**: Random Forest Regressor, chosen for its ability to handle non-linearities and rank feature importance.
- **Train/Test Split**: 80% training and 20% testing.
- **Evaluation Metrics**: MAE, MSE, and RMSE.

### 4. **Model Evaluation**
- Visualized actual vs predicted selling prices.
- Highlighted important features using bar plots.

### 5. **New Predictions**
Predicted selling prices for test data, showcasing model effectiveness.

### 6. **Recommendations**
- The trained model is saved as `car_price_prediction_model.pkl` for deployment.
- Suggestions for integration into car trading platforms as a price recommendation tool.

## Key Features of the Code
- **Modular Design**: Functions for data cleaning, visualization, model training, and evaluation.
- **Visualization**: Clear visual representations of key insights and model performance.
- **Scalability**: Can be extended to include additional features or new datasets.

## Prerequisites
1. Python 3.8+
2. Required Libraries:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
   - `scikit-learn`
   - `joblib`

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/car-price-forecasting.git
   ```
2. Navigate to the project directory:
   ```bash
   cd car-price-forecasting
   ```
3. Run the Python script:
   ```bash
   python car_price_forecasting.py
   ```

## Example Output
### Predicted Selling Prices for New Test Data:
```json
[694596.67, 831950.00]
```

## Future Enhancements
- Incorporate additional features like car condition and service history.
- Explore alternative algorithms like Gradient Boosting or XGBoost.
- Implement a web-based interface for user interaction.

## Contributing
Contributions are welcome! Feel free to submit a pull request or raise an issue for any suggestions or improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
