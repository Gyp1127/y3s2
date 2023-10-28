# Classification Models
### Suggestion: Look at the intuition of the models and how you would construct it from scratch

### Types of Machine/Statistical Learning

1. <details>
   <summary>What are the primary types of machine/statistical learning discussed?</summary>
   
   - Supervised Learning
   - Unsupervised Learning
   - Reinforcement Learning
   </details>
   
2. <details>
   <summary>What is supervised learning?</summary>
   
   Training data consists of inputs and outputs (i.e., a “supervisor” to tell some correct answers...). The goal is to build a model that predicts the output (dependent variable) from a given set of inputs (predictors).
   </details>

3. <details>
   <summary>What are the two types of problems in supervised learning?</summary>
   
   - Regression (output is a continuous variable)
   - Classification (output is a discrete variable)
   </details>

4. <details>
   <summary>Define Unsupervised Learning.</summary>
   
   There is no training data in unsupervised learning. The model is built from relationships between properties.
   </details>

5. <details>
   <summary>What is the goal of reinforcement learning?</summary>
   
   Agents take action in an environment, receive a reward, and update their strategy to maximize this reward over a horizon.
   </details>

6. <details>
   <summary>What are the synonyms used for the input variables in supervised learning?</summary>
   
   - Predictors
   - Independent variables
   - Input variables
   - Features
   </details>

7. <details>
   <summary>How are regression and classification problems differentiated in terms of their outputs?</summary>
   
   Regression problems have outputs that are continuous variables, while classification problems have outputs that are discrete variables.
   </details>

8. <details>
   <summary>How is linear regression useful?</summary>
   
   It's useful for predicting a quantitative response and understanding other methods. It assumes that the true function is linear or can be approximated by a linear function.
   </details>

9. <details>
   <summary>What is the objective of linear regression?</summary>
   
   The objective is to minimize the Residual Sum of Squares (RSS).
   </details>

10. <details>
    <summary>How can one interpret the linear regression equation?</summary>
    
    The coefficients represent the change in the response variable for a one-unit change in the predictor, keeping other predictors constant.
    </details>

11. <details>
    <summary>What provides an intuitive understanding of R-squared in linear regression?</summary>
    
    R-squared measures the proportion of the variance for the dependent variable that's explained by independent variables in a regression model.
    </details>

12. <details>
    <summary>How does gradient descent work in the context of linear regression?</summary>
    
    It starts with a guess for the coefficients, computes the direction of the gradient, moves some distance in that direction, and repeats the process until the optima is reached.
    </details>

13. <details>
    <summary>What is logistic regression used for?</summary>
    
    It's used for predicting a qualitative response, specifically when the response takes two values, such as 0 and 1.
    </details>

14. <details>
    <summary>Why can't probabilities in logistic regression be negative or more than 1?</summary>
    
    Probabilities represent the likelihood of an event occurring and must be between 0 and 1.
    </details>

15. <details>
    <summary>How does logistic regression ensure probabilities lie between 0 and 1?</summary>
    
    It uses the sigmoid transformation to restrict the response to between 0 and 1.
    </details>

16. <details>
    <summary>How is logistic regression related to odds?</summary>
    
    The odds can take a value between 0 (low probability) and infinity (high probability). For example, a probability of 0.2 implies odds of 1/4.
    </details>

17. <details>
    <summary>Describe the relationship between logistic regression and logit.</summary>
    
    The logistic regression has a logit that is linear in X. Increasing a predictor by one unit changes the log odds by its coefficient. The relationship between the predictors and the probability is not linear.
    </details>

18. <details>
    <summary>How is logistic regression interpreted?</summary>
    
    The coefficients represent the change in the log odds of the response for a one-unit change in the predictor, keeping other predictors constant.
    </details>

19. <details>
    <summary>What is the cost function in logistic regression?</summary>
    
    Estimates are chosen to maximize the likelihood (from a Stats/Econ/Finance view) or to minimize the Binary cross-entropy (from a Machine Learning view).
    </details>

20. <details>
    <summary>Provide an intuitive understanding of the cost function in logistic regression.</summary>
    
    The cost function measures the difference between the actual and predicted probabilities. A higher difference leads to a higher cost.
    </details>

21. <details>
    <summary>In the context of logistic regression, what challenges arise if one attempts to use linear regression for probability estimation?</summary>
    
    Linear regression might predict values less than 0 or greater than 1, which are not valid probabilities.
    </details>

22. <details>
    <summary>How does the logistic regression model restrict its response between 0 and 1?</summary>
    
    It uses the sigmoid transformation.
    </details>

23. <details>
    <summary>What is the significance of the odds in the context of logistic regression?</summary>
    
    The odds ratio represents the odds that an outcome will occur given a particular exposure, compared to the odds of the outcome occurring in the absence of that exposure.
    </details>

24. <details>
    <summary>What is the relationship between the logit and the predictors in logistic regression?</summary>
    
    The logit is linear in relation to the predictors.
    </details>

25. <details>
    <summary>Why is gradient descent used in linear regression optimization?</summary>
    
    It's used to minimize the Residual Sum of Squares (RSS) by iteratively adjusting the coefficients.
    </details>

26. <details>
    <summary>How is the goodness of coefficients in linear regression determined?</summary>
    
    By comparing the Residual Sum of Squares (RSS) with different values of coefficients.
    </details>

27. <details>
    <summary>How is the number of data points required for linear regression estimation determined?</summary>
    
    By observing the standard deviation of estimates as a function of data points.
    </details>

28. <details>
    <summary>What assumption is made behind the expansion in linear regression?</summary>
    
    The assumption is that the predictors are linearly related to the response variable.
    </details>

29. <details>
    <summary>How can one check if the obtained coefficients in linear regression are good?</summary>
    
    By observing the relation of RSS with different values of coefficients and through gradient descent.
    </details>

30. <details>
    <summary>What is the underlying assumption of linear regression regarding the true function?</summary>
    
    The assumption is that the true function is linear or can be approximated by a linear function.


# Model Evaluation
1. <details>
    <summary>What are the three types of metrics to compare two classifiers?</summary>

    - Threshold-based metrics
    - Threshold-free metrics
    - Domain specific metrics
</details>

2. <details>
    <summary>How do you predict labels given an estimated model?</summary>

    - Consider a threshold (e.g., 0.5)
    - Assign labels as per the threshold
</details>

3. <details>
    <summary>Define True Positives in the context of classification.</summary>

    True Positives (TP) refer to the number of cases that the classifier correctly predicts as fraudulent.
</details>

4. <details>
    <summary>Define False Positives.</summary>

    False Positives (FP) is the number of non-fraudulent cases that the classifier incorrectly predicts as fraudulent.
</details>

5. <details>
    <summary>Define True Negatives.</summary>

    True Negatives (TN) is the number of cases that the classifier correctly predicts as non-fraudulent.
</details>

6. <details>
    <summary>Define False Negatives.</summary>

    False Negatives (FN) is the number of fraudulent cases that the classifier incorrectly predicts as non-fraudulent.
</details>

7. <details>
    <summary>How can one compare two classifiers?</summary>

    By using accuracy, which can be looked at through mean mis-classification error or an accuracy score.
</details>

8. <details>
    <summary>What does the precision metric indicate?</summary>

    Precision is the fraction of positive instances amongst estimated positive cases. It is calculated as the ratio of True Positives to the sum of True Positives and False Positives.
</details>

9. <details>
    <summary>How is recall or sensitivity computed?</summary>

    Recall is the fraction of positive instances amongst actual positive cases. It is also known as sensitivity or True Positive Rate and is calculated as the ratio of True Positives to the sum of True Positives and False Negatives.
</details>

10. <details>
    <summary>Define False Positive Rate.</summary>

    The False Positive Rate is the fraction of incorrect positive predictions. It is calculated as the ratio of False Positives to the sum of False Positives and True Negatives.
</details>

11. <details>
    <summary>What is an ROC curve in the context of threshold-free metrics?</summary>

    The ROC curve is obtained by changing the threshold and plotting the False Positive rate against the True Positive rate.
</details>

12. <details>
    <summary>What influences the ROC curve?</summary>

    Differentiability influences the ROC curve, assuming a good classifier.
</details>

13. <details>
    <summary>How does peakness of distribution impact the ROC Curve?</summary>

    The ROC Curve is robust towards distribution peakness.
</details>

14. <details>
    <summary>Which is considered a better metric: ROC Curve or precision-recall curve?</summary>

    The ROC Curve is considered a better metric than the precision-recall curve.
</details>

15. <details>
    <summary>How do you select between two classifiers based on the ROC curve?</summary>

    One should choose the classifier that has a higher area under the curve (AUC). The AUC also provides a comparison with respect to a random classifier and a perfect classifier.
</details>

16. <details>
    <summary>In the context of domain-specific metrics, how many transactions can investigators manually check in a day?</summary>

    Investigators can only manually check a few transactions in a particular day.
</details>

17. <details>
    <summary>What is alert precision?</summary>

    Alert precision is the ratio of accurate alerts to the total number of alerts sent to investigators.
</details>

18. <details>
    <summary>Why might sending multiple alerts for the same card be considered a waste of time?</summary>

    Sending multiple alerts for the same card is wasteful because an investigator will typically check recent transactions from a card for which an alert has been issued.
</details>

19. <details>
    <summary>How is card alert precision defined?</summary>

    Card alert precision is the ratio of unique accurate card alerts to the total number of card alerts sent.
</details>

20. <details>
    <summary>What are the four outcomes in threshold-based metrics when comparing predictions against actual results?</summary>

    - True Positives: Actual: fraudulent, Estimate: fraudulent
    - False Positives: Actual: genuine, Estimate: fraudulent
    - False Negatives: Actual: fraudulent, Estimate: genuine
    - True Negatives: Actual: genuine, Estimate: genuine
</details>

21. <details>
    <summary>What is the significance of the threshold in threshold-based metrics?</summary>

    The threshold determines the point above which cases are labeled as positive and below which they are labeled as negative. Changing the threshold can impact the number of true positives, false positives, true negatives, and false negatives.
</details>

22. <details>
    <summary>What does a confusion matrix display?</summary>

    A confusion matrix displays the number of correctly and incorrectly predicted cases for both positive and negative labels.
</details>

23. <details>
    <summary>How can one determine which threshold is better in threshold-based metrics?</summary>

    By comparing the resulting values of true positives, false positives, true negatives, and false negatives, and other derived metrics such as accuracy, precision, and recall for each threshold.
</details>

24. <details>
    <summary>What are the concerns when considering metrics in isolation?</summary>

    Metrics in isolation may not provide a comprehensive understanding of the classifier's performance. For instance, a high precision may not be useful if recall is very low.
</details>

25. <details>
    <summary>What is an ROC curve used for in threshold-free metrics?</summary>

    An ROC curve is used to summarize the performance of a classifier across all thresholds by plotting the False Positive rate against the True Positive rate.
</details>

26. <details>
    <summary>What is the importance of the area under the ROC curve (AUC)?</summary>

    The AUC provides a scalar value representing the overall performance of a classifier. A higher AUC indicates better classifier performance.
</details>

27. <details>
    <summary>What is the goal of domain-specific metrics in fraud detection?</summary>

    The goal is to evaluate how effective the classifier is in the specific domain, such as how precise the alerts are that are sent to investigators.
</details>

28. <details>
    <summary>Why is it important to consider the distribution of classes when evaluating a classifier's performance?</summary>

    The distribution of classes can impact the classifier's effectiveness. For example, in imbalanced datasets, traditional metrics like accuracy might be misleading.
</details>

29. <details>
    <summary>How does differentiability impact the ROC curve?</summary>

    Differentiability, assuming a good classifier, influences the shape and position of the ROC curve.
</details>

30. <details>
    <summary>Why is the ROC curve considered robust towards distribution peakness?</summary>

    The ROC curve remains consistent in its representation of classifier performance, regardless of the peakness of the distribution of classes.
</details>
