Movie Rating Prediction

Overview

This project builds a machine learning model to predict movie ratings based on various attributes such as genre, director, duration, and cast. The dataset used is IMDb Movies India.

Dataset

Source: IMDb Movies India dataset

Features: Name, Year, Duration, Genre, Rating, Votes, Director, Actor 1, Actor 2, Actor 3

Target Variable: Rating (IMDb score)


Data Preprocessing

Extracted numeric values from Year and Duration

Converted Votes to a numeric format

Handled missing values using median (for numerical data) and mode (for categorical data)

Encoded categorical variables using Label Encoding


Feature Engineering

Director Success Rate: Average rating of movies directed by each director

Genre-Based Average Rating: Mean rating of movies within the same genre

Actor Influence: Average rating of movies featuring each actor


Model Selection

Used Random Forest Regressor for predicting movie ratings

Standardized numerical features

Split dataset into training (80%) and testing (20%) sets


Evaluation

Model performance evaluated using Mean Squared Error (MSE)


Repository Structure

Movie-Rating-Prediction/
│── data/                   # Store datasets (original & cleaned)
│── notebooks/              # Jupyter Notebooks for analysis & modeling
│── src/                    # Python scripts for preprocessing & modeling
│── README.md               # Project documentation
│── requirements.txt        # Dependencies
│── .gitignore              # Ignore unnecessary files

How to Run

1. Clone the repository:

git clone https://github.com/yourusername/Movie-Rating-Prediction.git
cd Movie-Rating-Prediction


2. Install dependencies:

pip install -r requirements.txt


3. Run the Jupyter Notebook or Python scripts to train and evaluate the model.



Results

The model successfully predicts IMDb ratings with reasonable accuracy, making it useful for estimating audience reception based on movie attributes.

Future Improvements

Try different machine learning models like XGBoost or Neural Networks

Improve feature engineering by considering more metadata (e.g., screenplay, production budget)

Optimize hyperparameters for better performance


Contributing

Feel free to fork the repository and submit pull requests for improvements
