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

- **Target Variables**
1. `h1n1_vaccine` - Whether respondent received H1N1 flu vaccine.
2. `seasonal_vaccine` - Whether respondent received seasonal flu vaccine.
Both are binary variables: 0 = No; 1 = Yes.

- **Independent Features**
1. `h1n1_concern` - Level of concern about the H1N1 flu.
0 = Not at all concerned; 1 = Not very concerned; 2 = Somewhat concerned; 3 = Very concerned.
2. `h1n1_knowledge` - Level of knowledge about H1N1 flu.
0 = No knowledge; 1 = A little knowledge; 2 = A lot of knowledge.
3. `behavioral_antiviral_meds` - Has taken antiviral medications. (binary)
4. `behavioral_avoidance` - Has avoided close contact with others with flu-like symptoms. (binary)
5. `behavioral_face_mask` - Has bought a face mask. (binary)
6. `behavioral_wash_hands` - Has frequently washed hands or used hand sanitizer. (binary)
7. `behavioral_large_gatherings` - Has reduced time at large gatherings. (binary)
8. `behavioral_outside_home` - Has reduced contact with people outside of own household. (binary)
9. `behavioral_touch_face` - Has avoided touching eyes, nose, or mouth. (binary)
10. `doctor_recc_h1n1` - H1N1 flu vaccine was recommended by doctor. (binary)
11. `doctor_recc_seasonal` - Seasonal flu vaccine was recommended by doctor. (binary)
12. `chronic_med_condition` - Has any of the following chronic medical conditions: asthma or an other lung condition, diabetes, a heart condition, a kidney condition, sickle cell anemia or other anemia, a neurological or neuromuscular condition, a liver condition, or a weakened immune system caused by a chronic illness or by medicines taken for a chronic illness. (binary)
13. `child_under_6_months` - Has regular close contact with a child under the age of six months. (binary)
14. `health_worker` - Is a healthcare worker. (binary)
15. `health_insurance` - Has health insurance. (binary)
16. `opinion_h1n1_vacc_effective` - Respondent's opinion about H1N1 vaccine effectiveness.
1 = Not at all effective; 2 = Not very effective; 3 = Don't know; 4 = Somewhat effective; 5 = Very effective.
17. `opinion_h1n1_risk` - Respondent's opinion about risk of getting sick with H1N1 flu without vaccine.
1 = Very Low; 2 = Somewhat low; 3 = Don't know; 4 = Somewhat high; 5 = Very high.
18. `opinion_h1n1_sick_from_vacc` - Respondent's worry of getting sick from taking H1N1 vaccine.
1 = Not at all worried; 2 = Not very worried; 3 = Don't know; 4 = Somewhat worried; 5 = Very worried.
19. `opinion_seas_vacc_effective` - Respondent's opinion about seasonal flu vaccine effectiveness.
1 = Not at all effective; 2 = Not very effective; 3 = Don't know; 4 = Somewhat effective; 5 = Very effective.
20. `opinion_seas_risk` - Respondent's opinion about risk of getting sick with seasonal flu without vaccine.
1 = Very Low; 2 = Somewhat low; 3 = Don't know; 4 = Somewhat high; 5 = Very high.
21. `opinion_seas_sick_from_vacc` - Respondent's worry of getting sick from taking seasonal flu vaccine.
1 = Not at all worried; 2 = Not very worried; 3 = Don't know; 4 = Somewhat worried; 5 = Very worried.
22. `age_group` - Age group of respondent.
23. `education` - Self-reported education level.
24. `race` - Race of respondent.
25. `sex` - Sex of respondent.
26. `income_poverty` - Household annual income of respondent with respect to 2008 Census poverty thresholds.
27. `marital_status` - Marital status of respondent.
28. `rent_or_own` - Housing situation of respondent.
29. `employment_status` - Employment status of respondent.
30. `hhs_geo_region` - Respondent's residence using a 10-region geographic classification defined by the U.S. Dept. of Health and Human Services. Values are represented as short random character strings.
31. `census_msa` - Respondent's residence within metropolitan statistical areas (MSA) as defined by the U.S. Census.
32. `household_adults` - Number of other adults in household, top-coded to 3.
33. `household_children` - Number of children in household, top-coded to 3.
34. `employment_industry` - Type of industry respondent is employed in. Values are represented as short random character strings.
35. `employment_occupation` - Type of occupation of respondent. Values are represented as short random character strings.
