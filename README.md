# DAY1
TASK OVERVIEW:
This is Task1 of ElevateLabs AI&ML internship,focused on learning Date Cleaning and the fundamentals of Data Preprocessing in Machine Learning.
The main goal is to prepare the Titanic dataset by cleaning and transforming it into a format suitable for machine learning models.

WHAT I LEARNED:
>How to identify and handle missing values using mean imputation and mode.
>How to encode categorical variables like Sex and Embarked.
>How to scale numerical features using StandardScaler.(mean=0,std=1)
>How to detect outliers using boxplots and remove them using IQR method.
>The importance of preprocessing in machine learning.

STEPS PERFORMED:
>Loaded the dataset and explore the missing values.
>Handled missing data:
1.Use mean imputation for Age,Fare(numericals)
2.Use mode for Embarked(categorical value)
3.Dropped Cabin column due to many missing values.
>Encoded categorical columns using label encoder.(encoding in alphabetical order)
>Standardized numerical columns to bring them to similar scales(range) so that all features contribute equally and ensure a better model training.
>Visulalized and removed outliers in Fare using boxplots and IQR.

Boxplot In Detail:
>It is generated using seaborn.
>data=df[num_cols] shows one boxplot per column in num_cols, which is the list of numerical features.
>These boxplots help identify outliers, which are extreme values that might confuse the model.
>Remove those outliers from the Fare column using IQR Method
Q1=25th percentile
Q3=75th percentile
IQR=Q3-Q1
outliers are pts outside the range [Q1 - 1.5*IQR, Q3 + 1.5*IQR]

>Verified that the final dataset has no missing values and is ready for ML.
