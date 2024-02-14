# Dementia Prediction Model
Made for Datathon 2.0
## Abstract
The first aspect of healthcare is understanding what disease a patient is suffering from.To do this the patient must undergo multiple different tests making it a time-consuming and expensive process overall This is where our Model steps in, it uses data from simple & affordable tests to quickly calculate the likelihood of having a disease and suggest further actions. The best part is that this can be used by either the lab or a normal user and provides a list of possible threats.

## Working
Our current prototype model relies mainly on behavioural data points to predict the likelihood of having Dementia such as: 
-Physical_Activity	
-Depression_Status
-Nutrition_Diet
-Sleep_Quality

## Why Behavioural Data?
Behavioural data is a powerful source of information that, when leveraged through machine learning (ML) models, proves to be highly effective in predicting diseases. Integrating big data analytics and ML algorithms allows for identifying intricate patterns and anomalies within an individual's behaviour. Daily habits, including food choices, respiration rate, and social behaviours, provides a holistic understanding of a person's health

Research indicates that ML applications can predict conditions such as diabetes, cancer, heart disease, autism, mental illness, Alzheimer's, and more, by examining daily habits like food choices, respiration rate, blood pressure, voice output, and social behaviours.


## Example of Practical Usage
Consider for example a patient A wishes to test themselves for Dementia. For this they will have to undergo the following:

Physical examination and laboratory tests. 
Cognitive testing. 
Mini-Mental Status Examination (MMSE) 
Alzheimer's Disease Assessment Scale-Cognitive (ADAS-Cog) 
Neuropsychological Testing. 
Radiological tests. 
Brain imaging techniques.

These tests are expensive and time-consuming and in the end if the patient tests negative the entire process is not productive.

###Now Consider that patient A uses our app, 
all they need to do is answer simple questions and undergo a simple inexpensive blood test.
Through this data our app will provide the likelihood of Dementia the patient has and then the patient can further decide to undergo proper tests.
Thus the patient saves time and resources and so does the lab, which can cater to more patients!


## Modeling

### Dataset 
we used the dementia_patients_health_data.csv from Kaggle. This dataset consists of multiple features which are used for predictions.
From this, we chose the features relating to Behavioural data.

### Model
We used CatBoost Classifier since we were dealing with a lot of categorical variables, alternatively, we could have used encoding but it would have been a lengthy process, we scaled our data and imputed it using simple imputer and built our pipeline using functions and for loops. Finally, we used stratified folds to increase model accuracy and conducted SHAP analysis to check for impact of features.

Then we added user input so it can provide a direct prediction based on likelihood!

# Steps to Use the model:
1. This model uses data from dementia_patients_health_data.csv so ensure its loaded correctly in your system
2. Use the model.ipynb file
3. Run the file and answer the questions
4. Wait for the model to load and run, (it will take approx 5 mins)
4. finally the model will provide you with an output as well as provide an output csv file

# Credits
Khush Trivedi
Dhruv Kapur
Samyak Bhansali
