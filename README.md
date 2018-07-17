This repo contains the following:

Folders:

**assets**
      - This folder contains a dataset obtained from PASSNYC, a non-profit that focuses on broadening educational opportunities for New York City’s underserved students
      - The dataset consists of NYC school data 

notebooks:

1. EDA:
    - In this notebook, I input the data and peform an extensive Data Cleaning and Exploratorty Data Analysis with several data visualizations

2. Model- Logistic Regression
    - Created a binary class logistic regression to predict student achievement rating 
    
3. Model- Random Forest and Grid Search CV 
    -  Created a Random Forest model with best estimators of max-depth=30 and n_estimators=5
    
4. Model- Neural Network
    - Here I explored a NN 
    
5. TPOT
    - Explored the TPOT package which optimizes machine learning pipelines 
    
**Executive Summary**
    My data was obtained from PASSNYC,a non-profit that focuses on broadening educational opportunities for New York City’s underserved students. The dataset from PASSNYC contained key features about schools, including location, school rigor, trust, community-family ties. My **goal** for the project was to find which key features have the biggest influence on student achievement rating of a school. 
    I ran two different **models**, Logistic Regression and Random Forest (with GridSearching). My target variable (Student Achievement Rating) was scored based on "Exceeding Target", "Meeting Target", "Approaching Target", "Not Meeting Target".
    1. In order to create my binary logistic regression model, I grouped 'exceeding' and 'meeting' target as 1 and then 'approaching' and 'not meeting' target as 0. I scored a 89% on my model, which was relatively higher than my original 74% baseline score.
    2. My second model was a RandomForest model with Grid Search. My model scored a 98%.
    
    From my findings, I found that the features I investigated were good predictors for Student Achievement Ratings. However, none of the features had very high or very low correlation coefficients. Some surprising findings were that Trust Rating did not have a strong correlation with Student Achievement Rating (coef: -.023).  Strong Family-Community Ties also did not have a strong correlation with Student Achievement Rating (coef: -.037). However, collaborative teachers and supportive environment, had a very small positive correlation with student achievement rating.  Interestingly enough, the schools with the highest economic need did not have the highest chronically absent percentage (missing 10% of school days ~18 in ~180 day school year). 
    
    This project was important to me because many times schools focus on simply increasing their students’ scores on exams and/or whether their curriculum is up to par with other schools. However, I was hoping to find other factors that were highly correlated that would increase the overall learning experience and success of students. 
    
    As for Next Steps, I would like to find gather more data from other cities to compare findings, continue fine tuning my models, perform more feature engineering, and explore other models (including Multi-class ordinal logistic regression). 

    
