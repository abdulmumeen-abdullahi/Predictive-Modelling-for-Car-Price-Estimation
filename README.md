# Predictive Modelling for Car Price Estimation

Incase the project file above return an error, you can alternatively access the file by clicking [here](https://nbviewer.org/github/abdulmumeen-abdullahi/Predictive-Modelling-for-Car-Price-Estimation/blob/main/Predictive%20Modelling%20for%20Car%20Price%20Estimation.ipynb).

## Overview of the Problem <br/>
The rapid expansion of the automobile industry has created challenges for car dealers and sellers in determining optimal selling prices for pre-owned cars. Key factors such as brand, mileage, fuel type, and transmission significantly impact a car's value. Mispricing can lead to financial losses or hinder sales. <br/>
This project aims to develop a predictive model to estimate car prices accurately, empowering sellers with actionable insights to maximize revenue opportunities. This aligns with the United Nations Sustainable Development Goal 9: Industry, Innovation, and Infrastructure, by fostering innovation through data-driven strategies to improve industry decision-making.


![image](https://github.com/user-attachments/assets/f36cbbb6-8022-4d91-b45e-259413113b05)


## Data Overview <br/>
The dataset, sourced from Kaggle, contains the following columns: <br/>
•	Car_Name: Name of the car model. <br/>
•	Year: Year of manufacture. <br/>
•	Selling_Price: Desired selling price of the car. <br/>
•	Present_Price: Current market price of the car. <br/>
•	Driven_kms: Distance covered by the car in kilometers. <br/>
•	Fuel_Type: Type of fuel used (Petrol/Diesel/CNG). <br/>
•	Selling_type: Individual seller or dealer. <br/>
•	Transmission: Gear system (Automatic/Manual). <br/>
**Note**: Selling prices were scaled by multiplying the values by 1,000 for better representation.

## Methodology

### 1. Data Preprocessing <br/>
•	Branding: Grouped car names into brands using a mapping dictionary. <br/>
•	Column Elimination: Dropped irrelevant columns like Car_Name, Year, Owner, and Present_Price. <br/>
•	Scaling: Multiplied the Selling_Price column values by 1,000. <br/>
•	Encoding: Used OneHotEncoder for categorical features.

### 2. Model Training <br/>
•	Data split into training (80%) and testing (20%) sets. <br/>
•	Established a baseline model using the mean value of Selling_Price. <br/>
**Trained multiple regression models**: <br/>
o	XGBoost Regressor (Best Performer) <br/>
o	Random Forest Regressor <br/>
o	Linear Regression <br/>
o	Decision Tree Regressor

### 3. Model Evaluation <br/>
•	XGBoost achieved the lowest Mean Absolute Error (MAE) of $1,263.1, outperforming all other models. <br/>
•	Baseline MAE: $3,445.8

### 4. Feature Importance <br/>
•	Extracted and visualized the top 7 features using a bar chart. <br/>
•	Insights: Fuel_Type (Diesel) emerged as the most critical predictor.

![download](https://github.com/user-attachments/assets/3b0c507c-b6c7-4c85-819b-124181920559)


## Results <br/>
•	Baseline MAE: $3,445.8 <br/>
**Model Performance**: <br/>
o	XGBoost: $1,263.1 <br/>
o	Random Forest: $1,632.6 <br/>
o	Linear Regression: $1,726.7 <br/>
o	Decision Tree: $1,306.9

![download](https://github.com/user-attachments/assets/e1a3b52d-a215-4771-a3a2-fe5cb0788b97)


## Feature Importance <br/>
Top predictors include Fuel_Type_Diesel, Selling_type_Individual, and Transmission_Manual. <br/>

## Interactive Dash Application <br/>
An interactive web app was created using Dash: <br/>
•	Inputs: Driven kilometers, fuel type, selling type, transmission, and brand. <br/>
•	Output: Predicted car price. <br/>
**Example Features**:
•	User-friendly sliders and dropdowns for data entry.
•	Real-time prediction on clicking "Predict Price".

![Predictive Modelling for Car Price Estimation](https://github.com/user-attachments/assets/f3b3ce11-dd6a-4755-a0f0-8a114072395f)


## How the Model Can Help Businesses <br/>
This car price predictive model empowers businesses to optimize pricing strategies, reduce inventory costs, and enhance customer trust by providing data-driven, accurate price estimates. It helps identify market trends, improve targeted marketing campaigns, and minimize financial risks, giving businesses a competitive edge in the automobile industry. By integrating this type of tool, companies can boost profitability, streamline operations, and position themselves as leaders in innovation and customer satisfaction.

**NOTE**: This project is a personal project to showcase my skills, and as such, the model is not intended for deployment in a real-world use case. For a more efficient and robust prediction model tailored to your business needs, please feel free to contact me for personalized services. <br/>
Abdullahi Olalekan Abdulmumeen <br/>
Applied Data Scientist <br/>
Olalekanabdulmumeen3@gmail.com
