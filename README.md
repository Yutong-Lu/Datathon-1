# Datathon-1
11-CHL5230-F23

## Research Questions

1. Is it possible to correctly predict for a patient’s lung cancer severity status based on patient parameters? (Age, Gender, Air Pollution, Alcohol Usage, Genetic Risk, Lung Disease, Obesity, Smoking, Passive Smoker, Chest Pain, Coughing of Blood)

2. If we ignore the label of lung cancer severities, can we cluster the patients with similar features into severities? Can we check this clustering and see if it is similar to the labels?

*Can we explore which explanatory variables to use in each research question?*

## Plans

### RQ1
1. Clean the data if needed
2. Separate the data into training and test sets
3. Perform K-NN on the training set (How to determine K?)
4. Check its performance on the test set

   General Practitioners/Family Doctors typically do not have access to such a wide breadth of data as seen in the study that we pulled this data from. It would be useful for doctors to be able to flag their patients for being at risk of lung cancer based on typical factors recorded on patient intakes. Variables to include: 'Age', 'Alcohol Usage', 'Obesity', 'Smoking'. Exclusion criteria for other variables was based on relevance, accessibility, and redundancy. (eg. Gender is irrelevant, Air Pollution data is difficult to obtain, Coughing Blood already marks a patient to do lung cancer tests/PFTs.) Lung cancer severity was converted into a binary variable where severity 0,1,2 => 1 (lung cancer present), and severity 3 => 0 (lung cancer absent). We also have a version of this code which does not convert severity to detection. Instead, the relevance of this file demonstrates that cancer severity can be predicted for using the easily obtainable variables with a 1% difference in accuracy compared to using all variables. (98% vs 97%)

   Debating on including symptom variables including 'Chest Pain' and 'Coughing of Blood' because different severities of these symptoms may lead to different lung cancer severities. Also might include "Lung Disease" because having lung disease does not directly mean a person has lung cancer. Passive smoking might be obtainable as the GP could obtain the number of people who smoked around the patient.

   Regarding the number of neighbours K in KNN, we tried a variety of K values and found that K=1 always gives the greatest accuracy and precision, but it may lead to overfitting of the model. We plotted accuracy vs K and precision score vs K with K ranging from 1 to 30, and found that the first large drop in accuracy or precision occurs when K increases from 3 to 4. *This might change depending on the variables we use.*

### RQ2
1. Separate the data into training and test sets
2. Drop the variable severity
3. Perform K-means clustering on the training set (Use K=4 because there are 4 levels of severities)
4. See if we get similar clustering as the variable severities


## Written Report

- Introduction: Explain the questions you aimed to answer with the data and their significance.

- Data Engineering Process: Describe how you cleaned and prepared the data and specify the datasets used.

- Analysis: Outline the learning and analysis techniques employed, along with the rationale behind their selection.

- Findings: Present your discoveries and insights.

- Conclusion: Summarize what health practitioners can infer from your team’s work.

- Individual Contributions: Highlight the contributions of each team member throughout the entire process.

- Code and Presentation: Host your Datathon materials, including notebooks and datasets, on GitHub. Share the GitHub project link in the report for easy access by the TA. Also, utilize Google Presentation to host your presentation and provide the public link in the report.

