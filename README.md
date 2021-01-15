# Introduction
This notebook performs ***Hypothesis Testing*** based on both sample means and sample proportions and performs ***regression analysis*** for medical data.
There are three data sources for analysis:
***Admissions***: Simulates administrative data where each row represents a unique admission to a hospital. 
***Lab***: Simulates results for patients who had laboratory testing (e.g. blood counts) in their admission.
***Transfusions***: Simulates information on patients who underwent a blood transfusion in their admission.
# Analysis 
1.  ***Data  Wrangling & Manipulation*** :Extracting data from all three sources and combining all sources into one data source using *admission_id* as the primary key, retaining all rows from Admissions data source(Left Join).

2.  ***Data Imputation:*** Imputing the missing features based on the type of the features(Categorical, Numerical)
    
3.  ***Hypothesis Testing on Sample Means:*** Determining if there is a significant difference in age between patients who had an RBC transfusion and patients that did not. 

4. ***Hypothesis Testing on Sample Proportions:*** Determining if there is a significant difference in sex between patients who had an RBC transfusion and patients that did not. 
    
5. ***Regression Analysis:*** Fitting a linear regression model using the *result_value* of the *“Platelet Count”* lab tests as the dependent variable and *age*, *sex*, and *hospital* as the independent variables. Interpreting the results.

6.  ***Visualizations :*** A plot that demonstrates the relationship between length_of_stay (*discharge date and time* minus *admission date and time*) and *charlson_comorbidity_index* using aggregation functions.

