# END-TO-END-DATA-SCIENCE-PROJECT

COMPANY: CODETECH IT SOLUTIONS

NAME: DEEKSHITH KUMAR

INTERN ID: CODHC14

DOMAIN: Data science

DURATION: 8 WEEKS

MENTOR: NEELA SANTHOSH

##DESCIPTION This script develops a customer churn prediction system using machine learning and FastAPI. It starts by importing necessary libraries such as pandas, numpy, scikit-learn, pickle, and FastAPI. The dataset is loaded from a CSV file, and preprocessing is performed by encoding categorical variables using LabelEncoder and pd.get_dummies(), while numerical features are standardized using StandardScaler. The dataset is split into training and testing sets, and a RandomForestClassifier is trained on the processed data. After evaluating the model’s accuracy using accuracy_score, the trained model, along with the scaler and feature names, is saved using pickle for later use.
The script then initializes a FastAPI application. Upon startup, it loads the saved model and preprocessing tools from the pickle file. A CustomerData class is defined using Pydantic to validate incoming requests, ensuring that inputs match the expected feature set. The /predict endpoint takes a list of numerical features as input, scales the data using the previously fitted StandardScaler, and predicts whether a customer is likely to churn or not using the trained RandomForestClassifier. The response includes the churn prediction (True or False) and the model’s accuracy.
Finally, if the script is run directly, it starts a FastAPI server using uvicorn, making the model accessible as an API. This implementation ensures that the churn prediction system is efficient, scalable, and ready for deployment in real-world applications.

##output

![Image](https://github.com/user-attachments/assets/93d9c5fa-d7ef-4595-b45d-69ada9f5899a)
