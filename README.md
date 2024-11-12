# Fire Weather Index Prediction

This project is a machine learning-based web application that predicts the Fire Weather Index (FWI) using environmental data. The FWI is a numerical indicator of fire potential in an area based on weather conditions, and it is widely used in forest fire prediction and prevention systems.

The application was built using multiple regression techniques to find the most accurate prediction model. A Ridge Regression model was selected for deployment based on its performance. The application provides an interactive user interface that allows users to input weather parameters, returning the predicted FWI score in real time. The project was deployed on AWS Elastic Beanstalk for scalability and accessibility.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Models Used](#models-used)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training and Selection](#model-training-and-selection)
- [Deployment](#deployment)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Overview

This project was created to provide a reliable, predictive model for determining fire risk levels using the Fire Weather Index (FWI). With nine key environmental inputs, the application generates an FWI score that can aid fire management services, researchers, and safety planners in risk assessment and decision-making. The model was trained using data from diverse weather conditions, applying various regression techniques to determine the most suitable approach for accurate prediction.

## Features

- **Interactive Input**: Users can enter 9 environmental parameters to get an FWI prediction.
- **Machine Learning Models**: Trained with various regression models, including Lasso, Ridge, and ElasticNet, with Ridge selected for deployment.
- **Web-Based Interface**: Built with HTML and CSS, providing a simple and intuitive interface.
- **AWS Elastic Beanstalk Deployment**: Hosted on AWS for secure, scalable access.

## Tech Stack

- **Frontend**: HTML, CSS
- **Backend**: Flask (Python)
- **Machine Learning Library**: Scikit-learn, Numpy, Pandas, Matplotlib, Seaborn
- **Deployment**: AWS Elastic Beanstalk

## Models Used

To find the best-performing model, the following regression models were trained and tested:

- **Multi-Linear Regression**: A simple linear approach considering all features.
- **Lasso Regression**: A regression analysis method that performs variable selection and regularization.
- **LassoCV**: Cross-validated Lasso to automatically find the best regularization parameter.
- **Ridge Regression**: Adds a penalty to the model for high coefficients, helping manage multicollinearity.
- **RidgeCV**: Cross-validated Ridge, used to identify the best regularization strength.
- **ElasticNet**: A combination of Lasso and Ridge regression.
- **ElasticNetCV**: Cross-validated ElasticNet to find the optimal mix of Lasso and Ridge penalties.

After testing these models, the Ridge Regression model was selected based on its balanced performance and suitability for the problem.

## Installation

### Prerequisites
Make sure you have the following installed:
- Python 3.11
- Numpy
- Pandas
- Matplotlib
- Seaborn
- Flask
- Scikit-learn
- AWS CLI (for deployment on AWS Elastic Beanstalk)

### Local Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/fire-weather-index-prediction.git
   cd fire-weather-index-prediction
