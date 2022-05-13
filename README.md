# Neural_Network_Charity_Analysis
**MODULE 10**

**CHALLENGE
 NEURAL NETWORKS **** Alphabet Soup**

1. **Overview of the analysis:**

We are working on a project with Alphabet Soup which is a charitable organisation. We have to use our knowledge of machine learning and neural networks, and use the features in the provided dataset to help them create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

There are more than 34,000 organizations that have received funding from Alphabet Soup over the years. Using Neural Networks we have to predict if these organisation are worth to get the donation from Alphabet Soup foundation.

1. **Results:**

- **Data Preprocessing**
  - What variable(s) are considered the target(s) for your model?
- IS SUCCESSFUL
  - What variable(s) are considered to be the features for your model?
- APPLICATION\_TYPE
- AFFILIATION
- CLASSIFICATION
- ORGANISATION
- INCOME\_AMT
- ASK\_AMT
  - What variable(s) are neither targets nor features, and should be removed from the input data?
- EIN
- NAME
- USE\_CASE
- STATUS
- SPECIAL\_CONSIDERATION

- **Compiling, Training, and Evaluating the Model**

  - How many neurons, layers, and activation functions did you select for your neural network model, and why?
- I have selected 120 neurons in First layer. As per the rule of the thumb neurons should be 2 to 3 times of the features. And we have 43 features in dataset.
- We have used ReLU activation function for input layer and hidden layers. The &quot;relu&quot; function is ideal for looking at positive nonlinear input data for classification or regression
- I have used sigmoid function for Output layer. The sigmoid function values are normalized to a probability between 0 and 1, which is ideal for binary classification.
  - Were you able to achieve the target model performance?
- No, I was not able to achieve a target predictive accuracy higher than 75%
- I can only achieved 73% of target predictive accuracy
  - What steps did you take to try and increase model performance?
- I tried to change the neurons, activation layer but at that point my target accuracy was just reaching 65% BUT when I created more bins for rare occurrences in columns then I was able to achieve the target accuracy of 73%

1. **Summary:**  Even after changing the neurons, adding more activation function and creating more bins for rare occurrences, we ended up with 73% accuracy and 0.55 Loss metric.

**Recommendation** : I would recommend to use SVM or Random Forest model over Neural Networks.

Both output and feature selection of random forest models are easy to interpret, and they can easily handle outliers and nonlinear data.

SVMs are less prone to overfitting because they are trying to maximize the distance, rather than encompass all data within a boundary.