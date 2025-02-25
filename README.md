# Churn Analysis & Prediction using Tableau & Machine Learning

## Overview

Customer churn is a critical issue for businesses, and analyzing churn patterns helps in developing retention strategies. This project consists of two key parts:

1️⃣ **Churn Analysis** : Utilizing Tableau dashboards to explore customer behavior, identify key factors contributing to churn, and visualize trends that impact customer retention.

2️⃣ **Churn Prediction** : Implementing a Machine Learning model (LightGBM) to classify customers as potential churners, predict churn probability, and evaluate model accuracy using real customer data.

## Objectives

  - Identify Key Drivers Behind Customer Churn: Analyze customer data to pinpoint the primary factors contributing to churn.
  - Segment Customer Profiles: Classify customers according to their churn risk to understand which segments are most likely to leave the service.
  - Provide Data-Driven Recommendations: Develop actionable insights and strategies to help Databel reduce customer churn and improve customer retention rates.

## Tools and Technologies Used

  - **Tableau**: Data visualization, dashboards, and churn analysis.
  - **Python (Jupyter Notebook)**: Data preprocessing and modeling.
  - **LightGBM**: Machine learning model for churn prediction.
  - **Pandas & NumPy**: Data manipulation and processing.
  - **Git and GitHub**: For Version Control.

## Skills Demonstrated

  - Data Visualization – Tableau dashboards for churn insights.
  - Exploratory Data Analysis (EDA) – Identifying key churn drivers.
  - Machine Learning – Implementing a churn prediction model.
  - Feature Engineering – Selecting key variables for ML.
  - Model Evaluation – Analyzing model accuracy & performance.
  - Business Understanding – Applying data insights for decision-making.

## Part 1 : Churn Analysis

### Business Understanding

#### Problem Statement : 
   -  Databel, a telecom provider, is experiencing customer churn where users terminate their services and switch to competitors. As a Data Consultant, my task is to investigate the root causes behind customer churn and provide actionable insights. This analysis will help Databel reduce churn rates, enhance customer satisfaction, and strengthen its market position.

#### Goal :
   -  Reduce Churn Rates: Implement data-driven strategies to decrease the number of customers leaving Databel. Success in this goal will contribute to increased customer retention, improved revenue stability, and a stronger competitive position in the telecom market.

#### Objectives :
   - **Identify Key Drivers Behind Customer Churn**: Analyze customer data to pinpoint the primary factors contributing to churn.
   - **Segment Customer Profiles**: Classify customers according to their churn risk to understand which segments are most likely to leave the service.
   - **Provide Data-Driven Recommendations**: Develop actionable insights and strategies to help Databel reduce customer churn and improve customer retention rates.

#### Business Metrics :
   - **Churn Rate**

### Exploratory Data Analysis (EDA)

#### Dataset : 
   - The [Databel dataset](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Churn%20Prediction%20Analysis/predicted_dataset.csv) consists of 29 columns and 6687 records.

#### Decriptive Statistics 

**Insights** :

**1. The churn rate of Databel is 26.86%**

**2. Churn Category Reason** :

Almost half of all customer churning are related to ```the competitor category (44.82%).```

![Churn Category Reason](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Churn%20Category%20Reason.png)

**3. Churn Reason** :

Top 5 reasons of churn customer in Databel :
   - Competitor made better offer (29.25%)
   - Competitor had better devices
   - Attitude of support person
   - Don't know
   - Competitor offered more data

![Churn Reason](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Churn%20Reason.png)

**4. Geomap** :

The churn rate in ```California (CA)``` is the highest ```(63.24%)```.

![Geomap](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Geomap.png)
 
**5. Demographics** :

Churn rate for ```Senior group``` is 10% higher than average ```(38.22%)```.

![Demographics](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Demographics.png)

**6. Age Group** :

The age group of 80-85 year old have the highest churn rates ```(52%)``` but they contain the least of people ```(only 25 customers)```.

![Age Group](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Age%20Group%20vs%20Number%20of%20Customers.png)

**7. Churn Rate by Group of Customer** :

The lowest churn rate ```(5.6%)``` is a customer group consisting of 6 people and conversely, the highest churn rate ```(32.85%)``` is for customers who are ```Not in a Group.```

![Group of Customer](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Churn%20Rate%20by%20Group%20of%20Custome.png)

**8. Extra Charge Vs Churn Rate** :

Here Extra International Charges ```$33.64``` have higher Churn Rate than Extra Data Charges.

![Extra Charge Vs Churn Rate](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/Data%20Plan.png)

**9.  International Plan** :

Customers who an International Plan but do not actively make international calls have the highest churn rate (71.19 but fortunately, the number of customers in this group is the lowest (177 customers). In this group, there appears to be the highest average monthly charge ($33.12).

![International Plan](https://github.com/gautamnakum40/Churn-Analysis-Prediction-Tableau-ML/blob/master/Plots/International%20Plan.png)





