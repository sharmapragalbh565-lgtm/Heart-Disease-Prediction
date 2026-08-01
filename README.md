# Heart Disease Prediction using Random Forest Classification
# Objective
The objective of this project is to predict the presence of heart disease in patients based on various clinical parameters using a Random Forest classification algorithm, and to deploy the trained model as a REST API using Flask. The API is accompanied by a custom web interface styled with a vintage anatomy textbook theme.

# Dataset
Dataset: Heart Disease Prediction
Dataset
Source: Kaggle

Important

The dataset file heart.csv should be placed in the project root directory before running the model training script.

# Libraries Used
pandas - data loading and manipulation
scikit-learn - train/test split, Random Forest classifier, and evaluation metrics
joblib - model serialization
flask - REST API development
gunicorn - WSGI HTTP Server for deployment
# Methodology
Task 1: Data Preprocessing

Loaded the dataset and identified target variable (target), numerical features, and categorical features.
Verified that there are no missing values in the dataset.
Split the data into an 80% training set and a 20% testing set.

Task 2: Model Development

Built and trained an ensemble Random Forest Classifier with 100 estimators.
Evaluated the model using the Accuracy Score metric.
Serialized and saved the trained model as model.pkl.

Task 3: Flask API & Frontend Setup

Developed a REST API using the Flask framework in app.py.
Configured an endpoint (/predict) to accept patient clinical parameters as JSON input.
Built a fully responsive frontend UI (templates/index.html) using a vintage anatomy textbook theme (featuring arterial red and venous blue accents).
Ensured the API returns the prediction in JSON format and displays it dynamically on the frontend.

Task 4: GitHub & Render Deployment

Structured the repository with the necessary source code, trained model, and configuration files.
Deployed the Flask application as a live web service using Render.

# Results

Model	Accuracy 98.54%
# Conclusion
In this project, the Random Forest classifier achieved an exceptional accuracy of 98.54% on the test set, demonstrating its strong capability to capture complex, non-linear relationships within clinical parameters for heart disease prediction. Deploying the model using Flask and Render proved to be a valuable experience, although ensuring the correct environment configuration via requirements.txt and handling proper JSON payload structures presented minor challenges. These hurdles highlight the critical importance of MLOps. Developing a machine learning model is only half the battle; MLOps practices are essential for transitioning models from isolated environments into scalable, reliable, and accessible production APIs. Proper deployment strategies ensure that predictive models can consistently process real-world data and deliver actionable insights efficiently.
