# Machine-Learning-Project
# NYC Property Sales Analysis & Prediction
📌 Project Overview
This project analyzes real estate data from the New York City Department of Finance to understand property market trends and predict sale prices. Using a dataset of NYC property sales (nyc-property-sales.csv), the project involves extensive data cleaning, exploratory data analysis (EDA), feature engineering, and machine learning modeling to estimate property values.

📂 Dataset
The dataset contains records of property sales in New York City. Key steps in handling the data included:

Source: NYC Property Sales data (Rolling sales data).

Filtering: Focused on sales data from the last 5 years to ensure market relevance.

Cleaning: handled missing values, removed transactions with $0 sale prices (transfer of ownership without cash), and converted data types for analysis.

🚀 Key Features & Workflow
1. Data Preprocessing

Standardized column names and handled missing/null values.

Converted SALE DATE to datetime objects.

Filtered out non-market transactions (e.g., $0 sales) and outliers.

Encoded categorical variables (Borough, Neighborhood, Building Class).

2. Exploratory Data Analysis (EDA)

Distribution Analysis: Visualized the distribution of sale prices and square footage.

Correlation Analysis: Generated heatmaps to identify relationships between features like Gross Square Feet, Residential Units, and Sale Price.

Time Series: Analyzed sales trends over the past 5 years.

3. Machine Learning Models

Several regression models were trained and evaluated to predict property sale prices:

Linear Regression: Established a baseline for prediction.

Gradient Boosting (LightGBM): Used for capturing complex non-linear patterns.

Random Forest Regressor: Implemented to improve accuracy and handle overfitting.

Decision Tree & SGD Regressor: Tested for comparison.

4. Model Evaluation

Models were evaluated using metrics such as RMSE (Root Mean Squared Error) and R² Score.

Random Forest was identified as the best-performing model for this dataset.

Feature importance analysis highlighted key drivers of property prices (e.g., Square Footage, Location/Borough).

🛠️ Technologies Used
Python

Pandas & NumPy (Data Manipulation)

Matplotlib & Seaborn (Visualization)

Scikit-Learn (Modeling & Preprocessing)

LightGBM (Gradient Boosting)

📊 Results
The Random Forest Regressor provided the most robust predictions.

Key insights indicate that GROSS SQUARE FEET and location (BOROUGH) are the most significant factors influencing NYC property prices.

Future improvements could include integrating external economic indicators (e.g., interest rates) or using advanced ensemble techniques.
