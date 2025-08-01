# Car Price Predictor using Machine Learning
This project predicts the selling price of used cars based on various features using a Linear Regression model. It includes steps like data cleaning, exploratory data analysis (EDA), model training, evaluation, and deploying a user-friendly web interface using Flask.


### Features Used:
The model uses the following features to estimate the car’s selling price:
- Present Price – Price of the car when bought (in lakhs)
- Kms Driven – Total distance driven
- Fuel Type – Petrol, Diesel, or CNG
- Seller Type – Dealer or Individual
- Transmission – Manual or Automatic
- Owner – Number of previous owners
- Car Age – Derived from Year of Purchase


### Workflow:
1. Data Preprocessing
- Removed irrelevant columns (e.g., Car_Name)
- Converted Year into Car Age
- Handled categorical features using one-hot encoding
- Scaled continuous features where needed

2. EDA
- Checked for correlations using heatmaps
- Visualized feature distributions and relationships with the target (Selling_Price)

3. Model Building
- Split data into training and test sets (80-20)
- Trained a Linear Regression model using scikit-learn
- Saved the trained model using pickle

4. Model Evaluation
- Evaluated using R² Score, Mean Squared Error
- Observed good fit for linear relationships

5. Deployment
- Created a Flask web app (app.py)
- Built a front-end form using HTML (templates/index.html)
- Integrated model to accept user inputs and return predictions


### Technologies Used:
- Python, Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (Linear Regression)
- Flask (for web deployment)
- HTML/CSS (for user input form)
- Pickle (to save model)

