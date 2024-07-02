# Supervised Machine Learning Project

## Project Outcomes
For this project, I created a supervised learning model that will predict diabetes in a patient using a diabetes statistics dataset. The dataset included predicting variables (pregnancy, age, insulin, BMI, skin thickness, glucose, blood pressure, and pedigree function), and the outcome (diabetes). 

The modules used in this project include: pandas, numpy, matplotlib.pyplot, seaborn, and sklearn. 

I performed EDA, data pre-processing, feature engineering, and supervised learning techniques to display data visualizations with the goal of communicating the insights gained from this analysis. I also utilized appropriate metrics (accuracy, precision, recall, f1-score, ROC-AUC) to evaluate the model properly. 

Two models were trained and evaluated to compare and see which model is more appropriate for this dataset, based off the metric scores. I selected a binary classification model, and a random forest ensemble model. 

### Process
1.	Explore dataset to get a clear understanding of the relationships between variables and how they affect the outcome variable. 
2.	Start data pre-processing. Clean the data by checking for null/missing values, duplicates, and outliers.
3.	Start feature engineering – I created a feature that combines age and pregnancies, I wanted to look at how geriatric pregnancies could potentially affect a patient’s likelihood of getting diabetes.
4.	Train the models. 
5.	Evaluate the models.

Correlation between variables and outcome:
<img width="999" alt="image" src="https://github.com/issajojoke/ml-project-supervised-learning/assets/140217218/af8c8740-f291-441d-8079-9de8d32f05d3">

### Findings
I found that the random forest ensemble method yielded higher metric scores than the binary classification model, making it the more ideal model for this dataset. From analyzing the data, I’ve learned that glucose is the strongest predictor of diabetes. The new feature that I engineered (PregnanciesOver35) did not affect a patient’s likelihood of getting diabetes. Lastly, skin thickness and insulin have a positive relationship, these two variables are good predictors for each other.

Random forest evaluation results:
<img width="221" alt="image" src="https://github.com/issajojoke/ml-project-supervised-learning/assets/140217218/040c56e3-f177-4262-abe8-142da3d9dc87">

Binary classification evaluation results:
<img width="221" alt="image" src="https://github.com/issajojoke/ml-project-supervised-learning/assets/140217218/7ddb8117-d3b0-4199-b176-8404f18873f2">

Feature engineering results:
<img width="529" alt="image" src="https://github.com/issajojoke/ml-project-supervised-learning/assets/140217218/c934beb1-fd6d-484e-8918-386c06cd5ec5">


### Challenges
I found the workflow of this project to be quite difficult to grasp. It was hard for me to navigate what to do first. For example, I was unsure if I should split the data before scaling it. The imbalance within the dataset was also a challenge for me, the number of patients without diabetes versus patients with diabetes was doubled.  Removing all outliers was a difficult task, even when I increased the multiplier value, the outliers remained. However, I came to the realization that this is a real-life health dataset, and outliers exist. These outliers are representative of how variable these predicting factors can be for diabetic patients, so I decided to keep them in the dataset.

Final data set with acounted outliers:
<img width="692" alt="image" src="https://github.com/issajojoke/ml-project-supervised-learning/assets/140217218/e21fc97f-8f5c-46e1-b940-7c3ec5da8db2">


### If I had more time
I would’ve explored other ensemble models to see if there was a different model better suited for predicting the outcome of this dataset.


