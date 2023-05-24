# Seasonal_Vaccine_Prediction
### Overview
Seasonal vaccinations are crucial for safeguarding the public's health and halting the spread of dangerous diseases. Data science techniques have become effective resources in recent years for comprehending and forecasting vaccine uptake, which is essential for determining vaccination campaigns. The goal of this data science modeling research is to apply predictive analytics to estimate people's willingness to receive seasonal vaccinations.

The project is aware of the significance of precise predictions in comprehending the elements that affect vaccination adoption. It tries to create models that can accurately predict whether people would consent to vaccinations by utilizing data science approaches. These forecasting insights have the power to improve public health outcomes by guiding targeted treatments and enhancing immunization plans.
### Business Understanding
Designing successful vaccination plans in the context of seasonal vaccines requires a thorough awareness of the financial consequences and aspects. In order to maximize vaccination uptake and raise the acceptance of seasonal vaccines, this initiative aims to give stakeholders, including healthcare organizations, public health authorities, and legislators, with actionable knowledge.

In order to reach high immunization rates among target demographics, businesses and healthcare professionals must overcome many major obstacles. Organizations can modify their communication and outreach efforts to address potential obstacles and concerns by accurately forecasting vaccine uptake or refusal. This can involve creating carefully crafted marketing campaigns, engaging the community, and giving pertinent information to people who might be wary of vaccinations. Predicting vaccine adoption can also assist in planning resource allocation and distribution.
#### Problem Statement
The challenge is to create a prediction model that can anticipate people's acceptance or rejection of seasonal immunizations. For reducing the spread of infectious illnesses and ensuring the health of communities, vaccine adoption must increase. However, achieving high immunization rates is significantly hampered by vaccine reluctance and rejection. In order to inform targeted treatments and improve vaccination tactics, it is necessary to address the issue of accurately forecasting vaccine acceptance.
#### Main Objective
The objective of this investigation is to develop a model that can forecast a person's acceptance or refusal of the seasonal flu vaccine based on their history and behavioural characteristics.
#### Metric for Success
- The accuracy of the models will inform on their success or lack thereof. The ideal accuracy that the project is aiming for is 80%. 

#### Description/Summary of Dataset
The dataset was download from Driven Data as part of a project that aims at predicting how likely people are to receive the H1N1 and seasonal flu vaccines. The data was part of a 2009 National H1N1 Flu Survey and contains 35 features and 2 target variables. The sects of datasets are as showcased below.

- **For this project, the seasonal_vaccine column was used as the target variable because it did not have a lot of imbalance between its binary variables**

### Modeling
From the problem statement, it is clear that the project dealt with a classification problem, and therefore, the models chosen had to be classifiers. The goal of classification problems is usually to estimate the probability of an event occuring based on a set of independent features. 
In this project, the base model was chosen to be `Logistic Regression` because of its capability to handle classification problems with ease, and also the fact that its results are highly interpretable. 
However, the results of this base model were deemed to be less apt because there was a problem of underfitting. So, other models were employed, including the `Random Forest Classifier`, `Gradient Boosting Classifier`, and the `XGBoost Classifier`. These were employed so that the best model that yields the best scores could be found. 

- Below are confusion matrices of all the models showcasing how they performed:
1. Confusion Matrix from the Logistic Regression Model

![image](https://github.com/MandelaGit/Seasonal_Vaccine_Prediction/assets/113025548/a672f657-fffa-475a-80ea-0a6705ab1397)

2. Confusion Matrix from the Random Forest Model

![image](https://github.com/MandelaGit/Seasonal_Vaccine_Prediction/assets/113025548/82408e11-6bf9-48f4-8ce7-27e43453e80c)

3. Confusion Matrix from the Gradient Boost Model

![image](https://github.com/MandelaGit/Seasonal_Vaccine_Prediction/assets/113025548/b1585ad2-0414-4522-8cee-07f9211da133)

4. Confusion Matrix from the XGBoost Model

![image](https://github.com/MandelaGit/Seasonal_Vaccine_Prediction/assets/113025548/51fcc0d0-abd2-4fa9-9875-2d1fd401fb43)


### Evaluation
![image](https://github.com/MandelaGit/Seasonal_Vaccine_Prediction/assets/113025548/129371a2-85be-4b4e-acea-a49cc032199c)
- From the dataframe above, it is clear that Gradient Boosting and XGBoost happen to post the highest scores. Therefore, these two models are chosen as the best for the classification problem that was being handled. 
- However, it is crucial to note that the models' accuracy scores were just shy of the 80% accuracy score that was declared as the metric of success for this project.

### Conclusion and Recommendations
- The models developed from the dataset happen to have relatively high accuracy scores, and while this is a good thing for the dataset at hand, it can also present some questions. For example, would the models above offer the same predictions if the data were to be skewed a little? If, for example, the race statistics were to be tweaked a little, would the models offer the same predictions? Also, considering that the dataset was not a universal representation of a population, can the conclusions drawn be generalized? 
- So, while the models performed well with the data provided, the results might be different if the dataset is tweaked. However, from the dataset, the models happened to provide their best predictions. 

#### Recommendations
The models have painted a clearer picture of how people normally respond to vaccines and vaccine campaigns. From the four models reviewed, it has been established that the opinions regarding vaccines, people's concerns over certain conditions, the age one belongs to, and even the knowledge one has regarding a condition greatly influences one's decision to be vaccinated. The chart shown below helps to paint a clearer picture of which features happen to have a greater influence on people's decision to take seasonal vaccines. 
![image](https://github.com/MandelaGit/Seasonal_Vaccine_Prediction/assets/113025548/0344d663-9ced-4164-8e46-6209f41531ad)

Therefore, from the above, public health efforts should consider the following:
1. Sensitize the young people more regarding seasonal vaccines. 
2. Shape the public narrative regarding seasonal vaccines through campaigns on the importance of flu vaccine. 
