# Weather API + Weather Observations Machine Learning Exercise

This project demonstrates the use of a weather API to collect historical weather data and applies machine learning to predict future temperatures. It utilizes Python for API integration, data preprocessing, and training a k-NN regression model.

## Table of Contents
- [Features](#features)
- [Setup](#setup)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Sample Output](#sample-output)
- [Future Improvements](#future-improvements)

## Features
- Fetch historical weather data for the past six months using the WeatherAPI.
- Preprocess and merge historical data into a structured dataset.
- Use k-NN regression to predict tomorrow’s temperature based on recent weather trends.
- Outputs model accuracy and tomorrow's predicted temperature.

## Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/DDavis-CP/Weather_prediction_model.git
   cd Weather_prediction_model
Install dependencies:
bash
Copy
Edit
pip install -r requirements.txt
Set up your WeatherAPI key:
Create a .env file in the project root directory.
Add the following line to the file:
makefile
Copy
Edit
API_KEY=your_weather_api_key
Dependencies
Python 3.8+
Libraries:
requests
pandas
scikit-learn
python-dotenv
Install dependencies using:

bash
Copy
Edit
pip install -r requirements.txt
Usage
Run the script:
bash
Copy
Edit
python main.py
The script will fetch data, preprocess it, train a k-NN model, and output:
Model accuracy
Tomorrow's predicted temperature.
How It Works
Data Collection:

The script fetches historical weather data for the past six months using the WeatherAPI.
Data includes average temperature, precipitation, and cloud cover.
Data Preprocessing:

Encodes categorical features like cloud cover into numeric values.
Scales numerical features for better model performance.
Model Training:

Splits the dataset into training and testing sets.
Uses k-Nearest Neighbors (k-NN) regression to predict tomorrow's temperature based on recent weather data.
Prediction:

Predicts tomorrow's temperature using the trained model.
Sample Output
mathematica
Copy
Edit
Model Accuracy: 0.88
Predicted Temperature for Tomorrow: 25.08°F
Future Improvements
Support for multiple locations.
Enhanced model with additional features like wind speed or humidity.
Integration with a frontend for live weather predictions.
Use of advanced models like LSTM or XGBoost for improved accuracy.
