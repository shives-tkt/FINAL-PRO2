Step 1: Data Loading and Exploration
The dataset was loaded from the provided Google Drive link using Pandas.
Basic exploration (head(), info(), describe()) was performed to understand the data structure, types, and any potential missing values.
Step 2: Data Preprocessing
Handling Missing Values: Missing values in numerical columns were replaced using median imputation for simplicity and to minimize bias.
Encoding Categorical Features: Label Encoding was applied to convert categorical variables into numeric form.
Normalization: Continuous numerical features were scaled using StandardScaler to standardize the input for clustering and regression models.
Step 3: Clustering
Algorithm: K-Means clustering was used to group land parcels into five clusters based on numerical features.
Cluster Validation: The silhouette score was calculated to evaluate the quality of clustering.
Visualization: Clusters were visualized using pair plots, revealing relationships between the features within each cluster.
Step 4: Regression Modeling
Feature Selection: Predictor variables (X) were separated from the target variable (Yield).
Train-Test Split: The dataset was split into 80% training and 20% testing subsets.
Model Training: A Random Forest Regressor was used to predict yield based on the selected features.
Evaluation:
Mean Squared Error (MSE): Assessed the model's predictive error.
R-squared (R²): Measured how well the model explains variance in the yield data.
Step 5: Visualization
A scatter plot of actual vs predicted yields was created to visually compare model performance. This plot highlighted the alignment (or deviation) of predictions from actual values.
Step 6: Saving the Model
The trained Random Forest model was saved as a .pkl file using Joblib for future deployment and reuse.
Step 7: Documentation
A README.md file was created to document:
Project overview.
Steps to run the script.
Evaluation metrics (MSE and R²).
Files generated, including the trained model.
Project Highlights
Clustering Results: Five meaningful clusters identified, assisting in targeted recommendations.
Prediction Accuracy: The regression model demonstrated measurable accuracy, aiding yield optimization.
Visualization: Insights were made accessible through visual tools, helping in decision-making.
