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

