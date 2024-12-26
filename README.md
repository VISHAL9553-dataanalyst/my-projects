# my-projects
Flight Price Prediction using ML

 Flight Fare Prediction

## Overview
Flight ticket prices are highly dynamic and can fluctuate drastically based on various factors. This project leverages machine learning techniques to analyze and predict flight ticket prices. By building and comparing multiple regression models, this project provides a predictive solution for estimating flight prices, aiding both airlines and travelers in better planning.

---

## Features
The dataset includes the following features:

1. **Airline**: Different airlines such as Indigo, Jet Airways, Air India, etc.
2. **Date_of_Journey**: The date when the journey starts.
3. **Source**: Starting point of the journey.
4. **Destination**: Endpoint of the journey.
5. **Route**: The route taken during the journey.
6. **Arrival_Time**: Arrival time at the destination.
7. **Duration**: Total travel time of the flight.
8. **Total_Stops**: Number of stops during the journey.
9. **Additional_Info**: Additional flight-related information.
10. **Price**: Target variable, representing the flight fare.

---

## Dataset
- **Source**: Provided dataset `Flight_Fare.xlsx`
- **Size**: 11 features and 10,683 records.
- **Preprocessing**: Includes handling missing values, feature encoding, and outlier detection.

---

## Project Structure

```plaintext
├── Flight_Fare_Prediction.py  # Main script for analysis and modeling
├── Dataset
│   └── Flight_Fare.xlsx      # Dataset used for training and testing
├── README.md                 # Project documentation
├── Results
│   └── Model_Evaluations.md  # Evaluation metrics and comparisons
```

---

## Setup and Installation

### Prerequisites
Ensure you have Python 3.8 or higher installed along with the required libraries.

### Libraries
The following libraries are used in this project:

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
- xgboost
- sweetviz

### Installation
Clone the repository and install the required libraries:

```bash
$ git clone https://github.com/your-repository-url.git
$ cd flight-fare-prediction
$ pip install -r requirements.txt
```

---

## Usage
1. Load the dataset by placing `Flight_Fare.xlsx` in the dataset folder.
2. Run the `Flight_Fare_Prediction.py` script to preprocess the data, analyze it, and build the prediction models:

```bash
$ python Flight_Fare_Prediction.py
```

3. Review model performance metrics and predicted values.

---

## Model Evaluation

The project implements and evaluates the following regression models:

- **Linear Regression**
- **Lasso Regression**
- **Ridge Regression**
- **Random Forest Regressor**
- **Decision Tree Regressor**
- **AdaBoost Regressor**
- **Gradient Boosting Regressor**
- **XGBoost Regressor**
- **Support Vector Regressor (SVR)**
- **K-Nearest Neighbors (KNN)**

### Metrics Used
1. R2 Score
2. Mean Absolute Error (MAE)
3. Mean Squared Error (MSE)
4. Root Mean Squared Error (RMSE)
5. Adjusted R2 Score

---

## Results
- The **Random Forest Regressor with Hyperparameter Tuning** achieved the best R2 score of ~85%.
- Key insights include:
  - Jet Airways Business class tickets tend to have the highest fares.
  - Ticket prices are highest for journeys originating from Bangalore.

Detailed evaluation metrics for all models are available in the `Results` directory.

---

## Contributing
Contributions are welcome! Please fork the repository and create a pull request for any changes or improvements.

---

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.

---

## Acknowledgments
- Special thanks to the creators of the dataset.
- Tools and libraries used include SweetViz for exploratory data analysis and Scikit-learn for modeling.
