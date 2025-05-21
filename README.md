This project explores a structured approach to cleaning, analyzing, visulaizing and applying machine learning models to a house prices dataset containing over 21,000 records.
Data Source: https://www.kaggle.com/datasets/harlfoxem/housesalesprediction?select=kc_house_data.csv
Key Topics: EDA, Data Cleaning, Scaling, PCA, K-means,Linear Regression, Apriori, Elbow Method, Feature Engineerig, Visualization.

****WorkFlow*****
•	EDA and Data Cleaning:
•	(EDA)first, got to know the data by checking the numbers of rows and columns.
•	(EDA)checked the min and max values in each column to get a sense of their ranges and if there's any outliers
•	(Nulls)started by checking for null values in each column, found none.
•	(Data cleaning)then, seaparated numeric columns in a separate dataframe for numeric-only operations.
•	(EDA)then created a heatmap matrix to find the correlations among feautres.
•	(Data Cleaning)cleaned inconcisistenies, like a fractional "number of rooms" values.
•	(Data Cleaning)Checked for imbalances in the dataset, found classes fairly distributed across median.

Linear Regression:
•	(Feature selection)Removed poorly correlated features to the target variable to avoid noise.
•	(train-test split)Split the data into 30% testing and 70% training.
•	(Scaling)Scaled the numeric data for better performance.
•	(Model Evaluation)Ran the model, intitillay got 50% accuracy.

Refining Linear Regression to 93% accruacy:
•	(Dimension Reduction)combined highly-correlated features into 1 dimenion that gives the same information game but reduces dimensions.
•	(Normalization) Used Log(target value) instead.
•	(Feature Engineering)converted wide-scale numeric features into a binary value, (0/1) indicating either above or below average.
•	Ran the model agian and got better results.

K-Means:
•	(Elbow Method)Performed Elbow Method to find the optimal k.
•	(PCA)Appplied PCA for dimensionality reduction.
•	(Visulization)ran the model and visualized the results.

Apriori Algorithm:
•	Categorized all Features into "High", "Low" and "AVerage" using the mean of each feature.
•	Generated all Association Rules with Support, Confidence and Lift.

Recovery:
created back-ups before every major change in the dataset.

