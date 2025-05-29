# Predict Calorie Expenditure

This is a small personal project built around the "Predict Calorie Expenditure" playground competition on Kaggle. The goal is to predict how many calories were burned during a workout based on various input features using various machine learning models.

## Task Description

The task is a supervised regression problem. Based on provided biometric and workout-related features, the objective is to predict the number of calories burned during physical activity.

### Steps Performed

1. **Data Exploration & Cleaning**  
   - Load the dataset  
   - Check for missing values  
   - Explore distributions and correlations  

2. **Feature Scaling & Preprocessing**  
   - Applied MinMaxScaler to standardize numeric features  
   - Ensured consistent input range for distance-based models  

3. **Model Training & Evaluation**  
   - Trained multiple machine learning regressors:  
     - Random Forest  
     - Gradient Boosting  
     - MLP Regressor  
     - K-Nearest Neighbors  
     - XGBoost  
   - Evaluated models using Root Mean Squared Error (RMSE)  

4. **Comparison of Model Performance**  
   - Visualized and compared performance using RMSE scores  

## Dataset Description

The dataset consists of biometric and exercise-related features for individuals. Key columns include:

- `Gender`: categorical (Male/Female)  
- `Age`: in years  
- `Height`: in centimeters  
- `Weight`: in kilograms  
- `Duration`: workout duration in minutes  
- `Heart_Rate`: average heart rate during workout  
- `Body_Temp`: average body temperature during workout (in °C)  
- `Calories`: target variable – calories burned  

## Model Performance (RMSE)

| Model                  | RMSE    |
|------------------------|---------|
| Random Forest          | 3.7824  |
| Gradient Boosting      | 3.6530  |
| MLP Regressor          | 3.6258  |
| KNN Regressor          | 4.2443  |
| XGBoost Regressor      | 3.6338  |

## Result

The best model achieved an RMSE of **3.6258** using an MLP Regressor. The model was selected based on its ability to generalize well to unseen data while keeping error minimal.

## Requirements

```
pandas  
numpy  
scikit-learn  
xgboost  
matplotlib  
seaborn  
```

## Useful Links

- 📂 [Kaggle Competition Page](https://www.kaggle.com/competitions/playground-series-s5e5)  
- 📊 [Kaggle Dataset Download](https://www.kaggle.com/competitions/playground-series-s5e5//data)  
- 💾 [File Storage (Google Drive, optional if used)](https://drive.google.com/drive/folders/1aL6xlvXNLezUMhxcw37T2Zb0i6fBJ0YH?usp=drive_link)  
