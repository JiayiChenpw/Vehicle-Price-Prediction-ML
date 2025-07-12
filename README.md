# Used Car Price Regression

## About the Project
This project predicts used car prices using various vehicle attributes such as brand, mileage, accident history, engine size, and more. We use a cleaned version of the Kaggle Playground Series S4E9 dataset (188,000+ entries) to explore price-related insights and apply multiple regression models for prediction.

## Key Features & Data Pipeline
- Performed **extensive feature engineering** on car specs using regular expressions and type mappings
- Created custom features including:
  - `mileage_per_year`, `is_luxury`, and normalized `engine_hp`, `engine_size`
- Conducted **exploratory analysis** to identify key factors:
  - Mileage, accident count, brand, and horsepower are highly correlated with price
- Ran **statistical hypothesis tests** to validate insights (e.g., color impact on pricing)
- Used **PyCaret** to benchmark multiple ML models:
  - Final model: LightGBM, selected via test performance and cross-validation

## Repository Structure
The repository includes:
- `used_car_regression.ipynb` – end-to-end pipeline with EDA, feature engineering, and modeling  
- `used_car_pipeline.py` – script version of the modeling pipeline  
- `CIS5450_Final_Presentation.pdf` – summary slides of project process and results  

## Dependencies
Install required packages:
```bash
pip install pycaret xgboost lightgbm
```

## To Run the Code
Open the notebook:
```bash
jupyter notebook used_car_regression.ipynb
```

Or run the script:
```bash
python used_car_pipeline.py
```

## Acknowledgments
- Dataset: [Kaggle Playground S4E9 – Used Car Price Regression](https://www.kaggle.com/competitions/playground-series-s4e9)  
- Course: CIS 5450 — Big Data Analytics @ University of Pennsylvania  
- Collaborators: jiayi Chen, Feng Jian, Amber Yan


