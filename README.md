# Built a model to identify fraudulent transactions on Credit Cards With a Decision Tree Classifier and a Support Vector Machine (SVM)

### Insights  
With a larger set of features, SVM perform better in comparison to Decision Trees.  
Decision Trees benefitted from feature selection and performed better.  
SVMs may require higher feature dimensionality to create efficient decision hyperplane.


I recently worked on a project to compare different machine learning models for identifying credit card fraud based on transaction history. The goal was to determine which model is more accurate in detecting fraudulent transactions.

Data Insights

During data exploration, I observed a significant class imbalance in the target variable, where:
🔹 1 represents a fraudulent transaction 
🔹 0 represents a legitimate transaction

To address this, I ensured the models accounted for the imbalance while training.

Experiments & Results

First Experiment: Using All Features

I trained both models using 29 out of the 31 available features (excluding time and the target variable). 
🔹 Decision Tree Classifier — ROC-AUC: 93.9% 
🔹 Support Vector Machine (SVM) — ROC-AUC: 98.6%

Second Experiment: Using Top 6 Correlated Features

I selected the six most correlated features with the target variable and retrained the models.
🔹 Decision Tree Classifier — ROC-AUC: 92.1% 
🔹 Support Vector Machine (SVM) — ROC-AUC: 97.2%

Key Takeaways:

✅ I observed that with large set of features, SVM perform better than Decision Trees
✅ Feature selection improved Decision Tree performance but had a slight impact on SVM. 
✅ SVMs may require higher feature dimensionality to create efficient decision hyperplane.
