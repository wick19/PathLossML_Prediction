# Path_loss_ML_Prediction
Machine Learning-Based Path loss Models For the UAV Air-to-Air (A2A) Prediction:

Synopsis:

Data Exploration and Cleaning:

Began by loading the dataset from a CSV file into a pandas DataFrame, checking its shape, and examining the first and last few rows to understand its structure.

Through methods like info() and isna().sum(), I ensured the dataset was clean and didn't contain any missing values.

Data Preprocessing:
Divided the data into features (like longitude, latitude, elevation, etc.) and the target variable (path loss).
To understand feature correlations, I created a heatmap using Seaborn, providing insights into which features might influence path loss.

Splitting the dataset into training and testing subsets using train_test_split allowed me to assess model performance accurately.
Model Training:
Leveraging scikit-learn, I trained various models including Linear Regression, K-Nearest Neighbors, Naive Bayes, Random Forest Classifier, and an Artificial Neural Network using MLPRegressor.
Standardized the data for models sensitive to feature scaling, ensuring fair comparisons.

Model Evaluation:

By generating confusion matrices, assessed each model's performance on the testing set, calculating metrics like precision, recall, and F1-score.
Grouping performance metrics into specific altitude ranges provided deeper insights into model behavior under different conditions.
Visualization:
Matplotlib and Seaborn were instrumental in visualizing data distributions, correlations, and model performance metrics.
Plotted various graphs including confusion matrices, bar charts for grouped metrics, and scatter plots for comparing model performance.
Path Loss Modeling:
Implemented two path loss models: Log-Distance Path Loss and Okumura-Hata Path Loss, showcasing how radio signal strength varies with distance and other factors.
Visualizations of these models helped in understanding the impact of distance and environment on signal propagation.
Advanced Visualization:
To predict radio channel behavior more comprehensively, created a 3D diagram using Matplotlib and NumPy, simulating Ray-Tracing to understand radio wave propagation in different scenarios.
Result :
Random Forest Classifier and K-Nearest Neighbors (KNN) demonstrated the highest training accuracies (84.74% and 86.74%, respectively).

Summary: Project involved a comprehensive analysis of urban models and UAV applications. I utilized various Python libraries such as pandas, NumPy, Matplotlib, Seaborn, and scikit-learn to process data, train machine learning models, evaluate their performance, and visualize results effectively. Additionally, I explored path loss modeling to understand radio channel behavior, demonstrating a deep understanding of data science techniques applied to real-world problems in urban modeling and UAV applications.
