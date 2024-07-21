# GDSC_ML_Final_Project
Notebook of my work to achieve 3rd place on Kaggle and 99.7% accuracy. The project is about utilizing NLP principles to classify real and fake news.
# Data Loading
1- Load training and testing data from CSV files.
2- Explore data using train_df.info() and train_df.describe().
3- Check for missing values using train_df.isnull().
# Feature Engineering - Subject Category
1- Create a new column subject_class to categorize subjects.
2- Define common subject categories (common_classes).
3- Use function classify_subject to assign a category based on string matching.
# Feature Engineering - Region
1- Create a new column region to assign the region.
2- Define function assign_region to assign the region based on keywords found in the title text.
3- Use assign_region to assign regions like "US", "Middle_East", etc.
# Date Parsing and Date Range Assignment
1- Define function safe_to_datetime to handle potential errors during date parsing using pd.to_datetime.
2- Assign date ranges (date_ranges).
3- Use function assign_date_range to assign a value from Range_1 to Range_19 based on date ranges.
4- If outliers are a small number within the same classification, give them Range_0.
# Model Training
1- Import machine learning libraries: sklearn and xgboost.
2- Split data into training and testing sets.
3- Define an XGBoost model.
4- Train the model on the training split.
# Evaluation
1- Evaluate model performance using metrics like accuracy, precision, recall, and F1-score.
2- Analyze results and identify areas for improvement.
