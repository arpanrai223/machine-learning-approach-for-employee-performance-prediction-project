## Employee Performance Analysis Project Documentation
# Overview
This project aims to analyze and predict employee performance based on various factors. The model is created using machine learning, specifically with the XGBoost algorithm, which has been chosen due to its superior performance in terms of R2 score compared to linear regression and random forest models.


# Installation and Setup
Clone the repository:
git clone [https://github.com/your-repo/employee_performance_analysis.git](https://github.com/abhinavomer/Employee_Performance_Analysis/edit/main/README.md)
cd employee_performance_analysis
Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
Install the required dependencies:

pip install -r requirements.txt
Run the Flask application:

python app.py
Open your web browser and navigate to:

http://127.0.0.1:5000/

# Model Development
- Data Preparation
- The dataset contains various features related to employee performance such as:

Quarter
Department
Day
Team
Targeted Productivity
SMV
Over Time
Incentive
Idle Time
Idle Men
No. of Style Changes
No. of Workers
Month
Model Selection
Three different models were tested:

- Linear Regression
- Random Forest
- XGBoost
- Among these, XGBoost provided the best R2 score, making it the chosen model for this project.

# Flask Application
Routes
Home (/): Displays the home page.
About (/about): Provides information about the project.
Predict (/predict): Displays the prediction form.
Submit (/submit): Shows the prediction result.
Prediction Endpoint (/pred): Handles form submissions and returns the prediction.
HTML Templates
base.html: The base template that includes Bootstrap and custom styles.
home.html: The home page template.
about.html: The about page template.
predict.html: The prediction form template.
submit.html: The prediction result template.
Static Files
styles.css: Custom CSS for styling the application.
Custom Styles
Custom styles are defined in the styles.css file and included in the base.html template. The background image is set directly in the base.html file using a URL.

# Project Structure
employee_performance_analysis/
│
├── app.py                  # Main Flask application
├── model.h5                # Serialized machine learning model
├── templates/              # HTML templates
│   ├── base.html           # Base template
│   ├── home.html           # Home page
│   ├── about.html          # About page
│   ├── predict.html        # Prediction form
│   ├── submit.html         # Prediction result
└── README.md               # Project documentation

# Model Training
The model was trained using the XGBoost algorithm, which is known for its high performance and accuracy. The data was split into training and testing sets, and various hyperparameters were tuned to optimize the model's performance.

# Model Serialization
The trained XGBoost model was serialized using the pickle library to be used in the Flask application for making predictions.

# Usage
Navigate to the Prediction Page:
Go to the prediction page by clicking the "Predict" link in the navigation bar.

Fill Out the Form:
Enter the required data into the form fields.

Submit the Form:
Click the "Submit" button to send the data to the server for prediction.

View the Prediction:
The prediction result will be displayed on the "Submit" page.
# Technologies Used
Python
Flask (web framework)
HTML/CSS (for the frontend)
Bootstrap (for responsive design)
XGBoost (machine learning model)
Pickle (for model serialization)

# Conclusion
This project provides a user-friendly interface for analyzing and predicting employee performance using machine learning. The XGBoost model, chosen for its high accuracy, is integrated into a Flask web application, allowing users to input data and receive predictions efficiently.



shuffle the data of this readme.md because it is copied from somwhere so make it unique