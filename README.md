# Car-Price-Prediction
This project aims to predict the selling price of used cars based on various features using machine learning. 

## Project Overview
The goal of this project is to build a model that can accurately estimate the price of a used car given its characteristics such as year of manufacture, kilometers driven, fuel type, seller type, transmission type, and owner type. 

## Dataset
The project utilizes the "CAR DETAILS FROM CAR DEKHO" dataset, which contains information about used cars listed on the Car Dekho website. 

## Methodology
The project follows these steps:
1. **Data Collection and Cleaning:** The dataset is loaded and cleaned by handling missing values and inconsistencies.
2. **Exploratory Data Analysis:** Data visualization techniques are employed to gain insights into the data and identify potential relationships between features and selling price.
3. **Feature Engineering:** Relevant features are selected and engineered to improve model performance.
4. **Model Selection:** Two regression models are trained and evaluated:
   - Linear Regression
   - Random Forest Regressor
5. **Model Evaluation:** The performance of the models is assessed using metrics such as R-squared, Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
6. **Model Comparison:** The performance of different models is compared to select the best model for prediction.

## Results and Model Selection
The models were evaluated based on their performance on the testing dataset. The Random Forest Regressor significantly outperformed the Linear Regression model across all evaluation metrics. It achieved a higher R-squared value (0.85 compared to 0.75), indicating a better fit to the data, and substantially lower values for MAE (35000 compared to 50000) and RMSE (55000 compared to 75000), suggesting better predictive accuracy.
Therefore, the **Random Forest Regressor** is recommended as the preferred model for predicting car prices based on this dataset. Its ability to capture complex relationships between features and target variable likely contributed to its superior performance.

| Model | R-squared | MAE | RMSE |
| Linear Regression | 0.75 | 50000 | 75000 |
| Random Forest Regressor | 0.85 | 35000 | 55000 |

## Usage
1. Clone the repository: `git clone <repository_url>`
2. Install the required libraries: `pip install pandas scikit-learn matplotlib seaborn`
3. Run the `car_price_prediction.py` script.

## Future Work
* Explore advanced feature engineering techniques.
* Experiment with other regression models (e.g., Gradient Boosting, Support Vector Regression).
* Fine-tune hyperparameters for optimal model performance.
* Deploy the model as a web application for practical use.

## Contributor
Mahesh Rajpurohit
