# Diabetes_health_indicator
To explore the factors associated with diabetes status (Diabetes_012) and identify key health, lifestyle, demographic, and socioeconomic predictors that may influence the risk of developing diabetes. This analysis aims to understand patterns in health behaviors, chronic conditions, and demographic characteristics that may contribute to diabetes, and to generate insights that can guide prevention and intervention strategies.

**INTRODUCTION**

Diabetes is among the most prevalent chronic diseases in the United States, 
impacting millions of Americans each year and exerting a significant financial 
burden on the economy. Diabetes is a serious chronic disease in which individuals 
lose the ability to effectively regulate levels of glucose in the blood, and can 
lead to reduced quality of life and life expectancy. After different foods are 
broken down into sugars during digestion, the sugars are then released into the 
bloodstream. This signals the pancreas to release insulin. Insulin helps enable cells within the body to use those sugars in the bloodstream for energy. Diabetes is generally characterized by either the body not making enough insulin or being unable to use the insulin that is made as effectively as needed.

Complications like heart disease, vision loss, lower-limb amputation, and kidney 
disease are associated with chronically high levels of sugar remaining in the 
bloodstream for those with diabetes. While there is no cure for diabetes, strategies like losing weight, eating healthily, being active, and receiving medical treatmentscan mitigate the harms of this disease in many patients. Early diagnosis can lead tolifestyle changes and more effective treatment, making predictive models for diabetesrisk important tools for public and public health officials.

The scale of this problem is also important to recognize. The Centers for Disease 
Control and Prevention has indicated that as of 2018, 34.2 million Americans have 
diabetes and 88 million have prediabetes. Furthermore, the CDC estimates that 1 in 5diabetics, and roughly 8 in 10 prediabetics are unaware of their risk. While there are different types of diabetes, type II diabetes is the most common form and its prevalence varies by age, education, income, location, race, and other social determinants of health. Much of the burden of the disease falls on those of lower socioeconomic status as well. 


**SCOPE**

PROJECT GOALS

To explore the factors associated with diabetes status (Diabetes_012) and identify 
key health, lifestyle, demographic, and socioeconomic predictors that may influence
the risk of developing diabetes. This analysis aims to understand patterns in health
behaviors, chronic conditions, and demographic characteristics that may contribute 
to diabetes, and to generate insights that can guide prevention and intervention 
strategies.

Describe diabetes prevalence across multiple demographic groups

Analyze lifestyle and health factors associated with diabetes

Investigate chronic conditions linked to diabetes

Examine barriers to healthcare access

This project will be able to answer some following questions:

DEMOGRAPHICS

- What is the prevalence of diabetes (Diabetes_012) in the dataset?

- How does diabetes status vary across demographic factors such as age, sex, 
education, and income?

- Which age groups show the highest proportion of diabetes?

LIFESTYLE

- Does BMI (Body Mass Index) differ significantly between diabetic and non-diabetic individuals?

- Is physical activity (PhysActivity) associated with lower diabetes prevalence?

- Does smoking (Smoker) status influence diabetes risk?

- Do heavy alcohol consumers (HvyAlcoholConsump) have different diabetes rates compared to non-heavy drinkers?

- Does fruit or vegetable consumption (Fruits, Veggies) relate to diabetes status?

CHRONIC DISEASE

- Is there an association between high blood pressure (HighBP) and diabetes?

- How does high cholesterol (HighChol) relate to diabetes status?

- Is there evidence that individuals with stroke or heart disease/heart attack have
higher rates of diabetes?

PHYSICAL HEALTH AND HEALTH CARE ACCESS

- Are mental health days (MentHlth), physical health days (PhysHlth) and difficulty 
walking (DiffWalk) more common among people with diabetes?

- Do individuals who have healthcare coverage (AnyHealthcare) and the inability to see
a doctor due to cost (NoDocbcCost) associated with higher diabetes prevalence?


**DATA**

diabetes _ 012 _ health _ indicators _ BRFSS2015.csv is a clean dataset of 253,680 
survey responses to the CDC BRFSS2015. 
The target variable Diabetes_012 has 3 classes. 0 is for no diabetes or only during pregnancy, 1 is for prediabetes, and 2 is for diabetes. 
There is class imbalance in this dataset. This dataset has 22 variables.

- Diabetes_012:
0 = no diabetes 1 = prediabetes 2 = diabetes

- HighBP
0 = no high BP 1 = high BP

- HighChol
0 = no high cholesterol 1 = high cholesterol

- CholCheck
0 = no cholesterol check in 5 years 1 = yes cholesterol check in 5 years

- BMI
Body Mass Index

- Smoker
Have you smoked at least 100 cigarettes in your entire life? [Note: 5 packs = 100 cigarettes] 0 = no 1 = yes

- Stroke
(Ever told) you had a stroke. 0 = no 1 = yes

- HeartDiseaseorAttack
coronary heart disease (CHD) or myocardial infarction (MI) 0 = no 1 = yes

- PhysActivity
physical activity in past 30 days - not including job 0 = no 1 = yes

- Fruits
Consume Fruit 1 or more times per day 0 = no 1 = yes

- Veggies
Consume Vegetables 1 or more times per day 0 = no 1 = yes

- HvyAlcoholConsump
Heavy drinkers (adult men having more than 14 drinks per week and adult women having more than 7 drinks per week) 0 = no 1 = yes

- AnyHealthcare
Have any kind of health care coverage, including health insurance, prepaid plans such as HMO, etc. 0 = no 1 = yes

- NoDocbcCost
Was there a time in the past 12 months when you needed to see a doctor but could not because of cost? 0 = no 1 = yes

- GenHlth
Would you say that in general your health is: scale 1-5 1 = excellent 2 = very good 3 = good 4 = fair 5 = poor

- MentHlth
Now thinking about your mental health, which includes stress, depression, and problems with emotions, for how many days during the past 30

- PhysHlth
Now thinking about your physical health, which includes physical illness and injury, for how many days during the past 30

- DiffWalk
Do you have serious difficulty walking or climbing stairs? 0 = no 1 = yes

- Sex
0 = female 1 = male

- Age
13-level age category (_AGEG5YR see codebook) 1 = 18-24 9 = 60-64 13 = 80 or older

- Education
Education level (EDUCA see codebook) scale 1-6 1 = Never attended school or only kindergarten 2 = Grades

- Income
Income scale (INCOME2 see codebook) scale 1-8 1 = less than $10,000 5 = less than $35,000 8 = $75,000 or more

**ANALYSIS/RESULTS**


**CONCLUSION**

**TAKE HOME / FURTHER RECOMMENDATION**
