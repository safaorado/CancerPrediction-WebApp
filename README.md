Breast Cancer Prediction App

A machine learning web application built with Streamlit that predicts whether a breast mass is benign or malignant based on cell nuclei measurements from a cytology lab.

Features

- Interactive Data Input: Use intuitive sidebar sliders to adjust 30 different cell nuclei measurements (Mean, Standard Error, and Worst values).
- Dynamic Visualization: Automatically generates a Plotly Radar Chart scaled from 0 to 1, comparing the selected measurements across different categories.
- Real-Time Predictions: Utilizes a pre-trained Logistic Regression machine learning model to instantly classify the tissue sample as Benign or Malignant.
- Confidence Scoring: Displays the exact probability percentages for both the benign and malignant classifications.

Technology Stack

- Frontend: [Streamlit](https://streamlit.io/)
- Machine Learning: [Scikit-Learn](https://scikit-learn.org/) (Logistic Regression, StandardScaler)
- Data Visualization: [Plotly](https://plotly.com/python/)
- Data Manipulation: [Pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/)

Url Link to the webapp
https://cancerprediction-webapp-fghguyhl3nbyhzbruubudu.streamlit.app/



Project Structure

```text
├── app/
│   └── main.py          # The main Streamlit application script
├── data/
│   └── data.csv         # The raw dataset used for baseline measurements
├── model/
│   ├── model.pkl        # The serialized Logistic Regression model
│   └── scaler.pkl       # The serialized StandardScaler object
├── train.py             # Script used to clean data and train the ML model
└── README.md
