Project overview:
This project aims to predict traffic flow using various regression-based machine learning models, providing smart insights for effective traffic management and planning in urban areas.

Dataset collection:
The dataset contains 48,120 records with following key features:
-> DateTime - Timestamp of vehicle count
-> Junction - Traffic junction identifier
-> Vehicles - number of vehicles observed
-> ID - Unique identifier(dropped during preprocessing)


1) Data preprocessing:
Loaded dataset in google colab
Removed Id column
Extracted new features (Year, Month, day, hour) from Datetime.

2) Exploratory Data Analysis (EDA):
Bar plots-> To show vehicle count junctions per year
Line plots-> For vehicle patterns by hour and day
Traffic Trends-> Visualized over time for each junction.

3) Model selection and training:
Applied three regression models.
Decision Tress Regressor
Random Forest Regressor
XGBoost Regressor

Training process:
Split data into training(80%) and testing (20%)
Applied GridSearchCV for hyperparameter tuining (especially XGBoost)

4) Evaluation and Visualization:
Visualized actual vs. predicted values
Compared models using:
-> Mean Squared Error (MSE)
->R² Score
Plotted error distributions using seaborn's distplot

5) Results
Random Forest and XGBoost performed the best
Accurate predictions of complex non-linear traffic patterns
Visualization showed good model alignment with real traffic flow.

key Takeaways:
Regression models can effectively predict traffic volumes
Features extraction from Datetime improves model performance
Visualization is critical for model validation and interpretation.


Tools and libraries used:
Python (NumPy, Pandas, Matplotlib, Seaborn)
Scikit-learn (DecisionTree, RandomForest, GridSearchCV)
XGBoost
Google Colab












