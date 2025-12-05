# Diabetes_health_indicator (DATA ANALYTICS PORTFOLIO PROJECT)
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
RESULTS AND INTERPRETATION
The dataset consist of 253680 observations(rows) and 22 variables (columns). There were no missing data. Diabetes status was coded as: 0 = No diabetes, 1 = Pre-diabetes, 2 = Has diabetes. Since the pre-diabetes is not a confirmed diabetes status, I decided to group it as non diabetes group, leaving diabetes to have binary values of 0 (no diabetes) and 1 (diabetes).

Statistical methods used include t-tests and chi-square tests to assess associations and differences across groups.

This project was able to analyse and answer the questions stated in the goals. Below are the results of each questions.

DEMOGRAPHICS
What is the prevalence of diabetes (Diabetes_012) in the dataset?
ANSWER: From our diabetes prevalence table, 13.9%(35346) of the entire population of our dataset has has diabetes. 84.2% (213703) does not have diabetes while 1.8% (4631) are in the prediabetes stage.

How does diabetes status vary across demographic factors such as age, sex, education, and income?
ANSWER: From our bar charts, we can conclude that: -For income and Education, diabetes status increases as income and education status increases. -For sex, diabetes are more common in females than in males, as females have the highest proportion of the population. -For age, diabetes values increases with age as the younger groups (18–24 and 25–29) had substantially lower prevalence.

Which age groups show the highest proportion of diabetes?
ANSWER: Diabetes prevalence increased with age. The highest proportion of diabetes was observed among individuals aged 70–74 years, followed by those aged 75–79 years. Younger groups (18–24 and 25–29) had substantially lower prevalence. From 75 - 79 and 80 - more had a slight decline maybe due to survivorship. Age is a strong non-modifiable risk factor.

LIFESTYLE
Does BMI (Body Mass Index) differ significantly between diabetic and non-diabetic individuals?
ANSWER: From the histogram and the values of the t-test performed with a tsat value of -99.9196, P-value: 0.000000, we can see that there is a significant difference between the BMI of diabetic and non-diabetic individuals. People with diabetes had higher BMI, suggesting overweight/obesity is linked to higher diabetes risk. Higher BMI is a strong modifiable risk factor for diabetes.

Is physical activity (PhysActivity) associated with lower diabetes prevalence?
ANSWER: Physical activity (1): lower prevalence, No physical activity (0): higher prevalence.From the chi-square test with values (chi2: 3539.42 p-value: 0.000000), association between Physical activity and Diabetes Prevalence is significant, also from the dataset and the bar chart, we can see that People who do physical activity tend to have lower diabetes prevalence and People who do not do physical activity have higher diabetes prevalence. Physical inactivity increases diabetes risk.

Does smoking (Smoker) status influence diabetes risk?
ANSWER: Diabetes prevalence was higher among smokers (16.29%) than non-smokers (12.06%), Prevalence shows: The difference is 4.24 percentage points (16.29 − 12.06 = 4.23). A chi-square test confirmed that this difference was statistically significant (χ² = 937.06, p < 0.001). This indicates that the prevalence of diabetes differs substantially between smokers and non-smokers. Therefore, smoking status has a strong influence on diabetes risk in this dataset. Smokers have higher diabetes prevalence.The extremely small p-value indicates this relationship is not due to chance. Smoking is significantly associated with higher diabetes risk.

Do heavy alcohol consumers (HvyAlcoholConsump) have different diabetes rates compared to non-heavy drinkers?
ANSWER:Diabetes prevalence was lower among heavy alcohol consumers (5.84%) compared to non-heavy alcohol consumers (14.42%), this is due to the proportion of heavy alcohol consumption population in our dataset. A chi-square test showed this difference to be statistically significant (χ² = 825.12, p < 0.001),indicating a strong association and statistical difference between heavy alcohol consumption and diabetes rates. Although heavy drinkers show lower diabetes prevalence, this result should be interpreted carefully, because:

Heavy drinkers may be younger.

They may have lower BMI.

They may differ in income, activity, or other confounders.

Some may under-report diabetes

People with diabetes often stop drinking

Some heavy drinkers may develop other health complications before diabetes appears.

Some datasets classify alcohol differently. So the pattern is statistical association, not necessarily causal protection. There is a significant association, but lower diabetes rates among heavy drinkers should not be interpreted as protective. Just because heavy drinkers have lower diabetes prevalence in your dataset does not prove alcohol reduces diabetes risk.

Does fruit or vegetable consumption (Fruits, Veggies) relate to diabetes status? ANSWER: Fruits Chi2 = 421.61, p < 0.000001 Very strong evidence that fruit consumption is associated with diabetes status. Vegetables Chi2 = 811.81, p < 0.000001 Even stronger evidence that vegetable consumption is associated with diabetes status. Statistically, both relationships are highly significant.

Fruits Population: Eating fruits = 160,898 Not eating fruits = 92,782

Vegetables Population: Eating vegetables = 205,841 Not eating vegetables = 47,839

Large sample sizes mean: Chi-square tests have very high statistical power This supports that the relationships are not only statistically significant but also practically relevant.

Fruits and diabetes People who do not eat fruits show ~23% higher diabetes prevalence (15.79 vs 12.86) Vegetables and diabetes People who do not eat vegetables show ~38% higher diabetes prevalence (17.99 vs 12.99)

The vegetable-consumption relationship is stronger, based on: -Higher prevalence gap -Higher chi-square statistic -Smaller veggie-eating group (47k) compared to fruit-eating group (92k), yet stronger effect

Fruit and vegetable consumption both show significant associations with diabetes status. Individuals who do not eat fruits have higher diabetes prevalence (15.79%) compared to those who do (12.86%). The effect is even stronger for vegetables: non-consumers have a diabetes prevalence of 17.99% compared to 12.99% among consumers. Chi-square tests confirm these associations are statistically significant (p < 0.000001). Given the large sample sizes, these findings provide strong evidence that lower fruit and vegetable intake is linked to higher diabetes prevalence in this population.

CHRONIC DISEASE
Is there an association between high blood pressure (HighBP) and diabetes?
ANSWER: There is a strong relationship between HighBP and diabetes. A chi-square test showed this relationship to be statistically significant (χ² = 17564.45, p < 0.001),indicating a strong association and statistical difference between HighBP and diabetes status.

How does high cholesterol (HighChol) relate to diabetes status?

ANSWER: There is a strong relationship between HighBP and diabetes. From our Chart and our Chi square test, the relationship is statistically significant indicating a strong association and statistical difference between High Cholesterol and diabetes status.

Is there evidence that individuals with stroke or heart disease/heart attack have higher rates of diabetes?

ANSWER: The relationship between Stroke/HeartDiseaseorAttack and Diabetes is significant after performing a chi-square test giving a very low p-values and high chi2 values.

PHYSICAL HEALTH AND HEALTH CARE ACCESS
Are mental health days (MentHlth), physical health days (PhysHlth) and difficulty walking (DiffWalk) more common among people with diabetes?

ANSWER: After performing a t-test method for both MentHlth and PhysHlth we got a very low value of p-value showing a strong relationship between both variables and diabetes status.

Do individuals who have healthcare coverage (AnyHealthcare) and the inability to see a doctor due to cost (NoDocbcCost) associated with higher diabetes prevalence?

ANSWER: Individuals who have access to healthcare coverage and who have access to see the doctor irrespective of cost tends to have a higher proportion of diabetes prevalence. Our Chi square test and our chart can show the relationship between both variables and diabetes status.

**CONCLUSION**
CONCLUSION
The analysis provides strong evidence that several lifestyle and demographic factors are associated with diabetes risk in the population. Across all variables, several consistent patterns emerge:

Non-modifiable risk factor:

Age: Older individuals show significantly higher diabetes prevalence.
Modifiable risk factors:

High BMI: Strongly linked to diabetes.

Physical inactivity: Higher diabetes prevalence in inactive individuals.

Smoking: Strong statistical association with higher diabetes.

Poor diet: Low fruit and vegetable intake associated with higher diabetes.

Chronic condition: Stroke, HighBP, High Cholesterol, HeartAttack/Disease associated with higher diabetes.

Physical Health Conditions: Difficult in walking, Physical health, mental health are associated with higher diabetes.

Health Care Access and Visiting the doctor irrespective of cost(NoDocBcCst) are associated with higher diabetes.

Diabetes risk increases sharply with age, especially in individuals aged 45+. BMI is significantly higher among diabetic individuals, identifying obesity as a major risk factor. Physical inactivity shows a strong association with increased diabetes prevalence. Smokers have significantly higher diabetes prevalence than non-smokers. Fruit and vegetable consumption are protective, showing lower diabetes prevalence among consumers.

Statistical tests (chi-square and t-test) consistently show that these relationships are significant and unlikely due to chance.

Overall, both lifestyle and demographic characteristics play important roles in diabetes status.

**TAKE HOME / FURTHER RECOMMENDATION**
Increase Physical Activity: Public health campaigns promoting daily exercise. Workplace and school physical activity programs.

Strengthen Smoking Cessation Programs: Integrate diabetes education into smoking-related health messaging. Provide support to help individuals quit smoking.

Improve Dietary Habits: Emphasize eating fruits and vegetables daily.Increase access to affordable produce in communities.

Focus Screening on High-Risk Age Groups: Encourage regular diabetes testing for adults aged 45+.

Carefully Interpret Alcohol Results: Do not recommend heavy drinking.Investigate confounding factors in further analyses.

Multi-factor Prevention Approach: Diabetes prevention programs should combine: Healthy diet, Physical activity, Weight reduction, Smoking cessation, Age-targeted screening.

**CHALLENGES AND LIMITATIONS OF THIS ANALYSIS**
This analysis faces several challenges, including confounding variables, self-reported behaviour bias, and the inability to establish causal relationships due to the cross-sectional nature of the data. Large sample sizes inflate chi-square significance, and binary coding oversimplifies complex behaviours such as diet and physical activity. Diabetes may also be underreported or undiagnosed. These limitations should be considered when interpreting associations between lifestyle factors and diabetes risk.
