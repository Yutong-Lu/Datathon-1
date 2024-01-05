# Lung Cancer Prediction and Severity Classification using KNN
## Authors: Myron Moskalyk, Yutong Lu, Feifan Xiang

**Datathon 1, CHL5230 Datathon 1, Dalla Lana School of Public Health**

### Introduction
- Explored machine learning techniques like KNN to support decision-making in public healthcare.
- Aimed to predict lung cancer presence and severity in patients using a dataset featuring healthy individuals and lung cancer patients.

### Data Engineering Process
- Conducted exploratory data analysis including pair plots and correlation matrices for two research questions.
- Chose features for each question based on correlations, creating separate datasets for presence prediction and severity classification.
- Split the dataset into 80% training and 20% test sets and standardized features for KNN.

### Analysis
- Employed KNN for both research questions, selecting optimal K values through accuracy, precision, and recall metrics.
- Conducted confusion matrix and classification report for each question's KNN models.

### Findings
#### Cancer Presence Prediction
- Achieved precision of 0.85 and 0.84, recall of 0.93 and 0.68 for cancer presence and absence respectively.
- The model exhibited high accuracy (0.85) and generalized well to unseen data.

#### Cancer Severity Prediction
- Obtained high precisions and recalls for different severity levels (0, 1, 2) ranging from 0.90 to 1.00.
- Best performance observed for predicting severity level 2.

#### Secondary Findings - Clustering Analysis
- Applied K-modes for clustering, finding that cancer and healthy patients tend to lay in the same cluster.
- Quadratic Discriminant Analysis yielded high precision of over 0.90.

### Conclusion
- The model for RQ 1 can assist in identifying potential lung cancer cases, while RQ 2 model performs best for high severity cases.
- Caution advised for moderate/low severity predictions, indicating potential reliability issues.

### Code and Presentation
- Google Slides Presentation: [Link to presentation](https://bit.ly/3LCbHur)

For a detailed understanding, kindly refer to the full report available in the provided GitHub repository.
