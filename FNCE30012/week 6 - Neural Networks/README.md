# Imbalance Learning
<details>
<summary>1. What is the purpose of imbalance learning?</summary>
Imbalance Learning is useful for domains where the number of examples for a class is skewed. For instance, in situations where the percentage of fraudulent transactions is around 0.02%. It addresses common issues in problems like claim prediction, default prediction, detection of rare diseases, and anomaly detection.
</details>

<details>
<summary>2. What challenges are often accompanied by imbalanced data?</summary>
a) Overall small size of minority class to learn from
b) Overlapping features between majority and minority class
c) Different clusters in minority label
</details>

<details>
<summary>3. What are the primary approaches to better handle imbalanced data?</summary>
Approaches include:
● Cost sensitive learning: Change the learning method to bias towards minority class
● Data level methods: Modify the training data to adjust the imbalance
</details>

<details>
<summary>4. What is cost sensitive learning?</summary>
In cost sensitive learning, the cost function of the learning method is modified. The penalty for mis-classification depends on the class and can be viewed as minimizing “conditional risk”. Costs are generally associated with classes.
</details>

<details>
<summary>5. How are costs associated in cost sensitive learning?</summary>
Costs can be defined using a cost matrix. For instance, labelling a fraudulent transaction as genuine will have a higher cost as opposed to labelling a genuine transaction as fraudulent.
</details>

<details>
<summary>6. How can the optimal prediction for an example be determined in cost sensitive learning?</summary>
Class that minimises the sum over all classes of the probability of a class times the cost associated with predicting another class. For binary classification, it involves calculations based on the cost matrix.
</details>

<details>
<summary>7. What is the cost of predicting a transaction as genuine?</summary>
It is the sum of the probability of the transaction being genuine multiplied by the correct classification cost plus the probability of the transaction being fraudulent multiplied by the incorrect classification cost.
</details>

<details>
<summary>8. How is the cost of predicting a transaction determined when costs are not explicitly known?</summary>
If the exact costs are unknown, the imbalance ratio can be used as a heuristic. The cost of a false negative is set to 1, and the cost of a false positive is set to the imbalance ratio.
</details>

<details>
<summary>9. What are resampling strategies in the context of imbalanced learning?</summary>
Resampling strategies involve modifying the dataset to reduce imbalance. The primary techniques include:
● Undersampling: Remove examples of the majority class
● Oversampling: Replicate or create new examples of the minority class
● Hybrid: Combine undersampling and oversampling methods
</details>

<details>
<summary>10. What is SMOTE?</summary>
SMOTE stands for Synthetic Minority Oversampling Technique. It creates new (synthetic) examples of the minority class by interpolating in the feature space. It involves randomly picking a positive example, finding its neighbors, and generating a new example between these instances. However, there's a caveat: it can aggregate specific clusters of the minority class.
</details>

<details>
<summary>11. Why is the detection of rare diseases considered a domain for imbalance learning?</summary>
The detection of rare diseases is an imbalanced learning domain because the instances of people having rare diseases (minority class) are significantly fewer than those not having them (majority class).
</details>

<details>
<summary>12. Why can simply having an imbalanced dataset not be enough to adversely affect the learning problem?</summary>
Imbalance in itself may not be sufficient to affect the learning adversely. Issues like a small size of the minority class to learn from, overlapping features between classes, and different clusters in the minority label can compound the problem.
</details>

<details>
<summary>13. How does cost sensitive learning view the misclassification penalty?</summary>
Cost sensitive learning views the misclassification penalty as minimizing “conditional risk”, where the penalty depends on the class being predicted.
</details>

<details>
<summary>14. In what situations would the cost of labeling a genuine transaction as fraudulent be higher?</summary>
Situations like sending a patient with a rare infectious disease home or labeling a fraudulent transaction as genuine would typically have higher costs associated with them due to the potential severe consequences.
</details>

<details>
<summary>15. What is the significance of the imbalance ratio in cost sensitive learning?</summary>
The imbalance ratio serves as a heuristic when exact costs are unknown. It helps determine the relative cost of false negatives to false positives based on the distribution of classes in the dataset.
</details>

<details>
<summary>16. What are the potential benefits and risks of undersampling and oversampling?</summary>
Undersampling can help in reducing the majority class to balance the dataset, but it might lead to loss of important information. Oversampling, on the other hand, can amplify the minority class, but there's a risk of overfitting to the minority class.
</details>

<details>
<summary>17. How does SMOTE use the feature space to create synthetic examples?</summary>
SMOTE operates in the feature space by randomly selecting a positive example, finding some of its neighbors, and generating a new synthetic example that lies between these instances.
</details>

<details>
<summary>18. What is the potential caveat of using SMOTE?</summary>
SMOTE can aggregate or overemphasize specific clusters of the minority class, which might not be representative of the true distribution.
</details>

<details>
<summary>19. Why is cost sensitive learning considered an approach to handle imbalanced data?</summary>
Cost sensitive learning biases the learning method towards the minority class by adjusting the misclassification penalties, making it suitable to handle datasets where one class is significantly underrepresented.
</details>

<details>
<summary>20. What is the role of a cost matrix in cost sensitive learning?</summary>
A cost matrix defines the costs associated with predicting one class when the true class is another. It helps quantify the penalties associated with different types of misclassifications.
</details>

# Neural Networks

<details>
<summary>1. What is the formula for the sigmoid function?</summary>

Answer: \( s(x) = \frac{1}{1 + e^{-x}} \)
</details>

<details>
<summary>2. How is logistic regression defined mathematically?</summary>

Answer: \( s(x) = \frac{e^{f(x)}}{1 + e^{f(x)}} \) where \( f(x) = w_0 + w_1x_1 + w_2x_2 + \dots + w_nx_n \)
</details>

<details>
<summary>3. What is a Neural Network Unit?</summary>

Answer: A Neural Network Unit is composed of a linear transformation followed by a non-linear transformation.
</details>

<details>
<summary>4. How do Neural Networks differ from Linear Regression and Logistic Regression?</summary>

Answer: Neural Networks are composed of multiple layers and units which can represent complex non-linear functions, whereas Linear and Logistic Regressions are simpler models.
</details>

<details>
<summary>5. What is a computation graph in the context of Neural Networks?</summary>

Answer: A computation graph visualizes the operations and their sequence in a neural network, typically using nodes to represent operations and edges to represent the data flow.
</details>

<details>
<summary>6. How is an AND Gate represented in a Neural Network?</summary>

Answer: For inputs \( x_1 \) and \( x_2 \), the output is 0 if \( x_1 + x_2 - 1 \leq 0 \) and 1 if \( x_1 + x_2 - 1 > 0 \).
</details>

<details>
<summary>7. How is an OR Gate represented in a Neural Network?</summary>

Answer: For inputs \( x_1 \) and \( x_2 \), the output is 0 if \( x_1 + x_2 \leq 0 \) and 1 if \( x_1 + x_2 > 0 \).
</details>

<details>
<summary>8. How is an XOR Gate represented using a Neural Network?</summary>

Answer: An XOR Gate cannot be represented by a simple linear model. In a neural network, multiple layers with specific weight configurations are required to represent the XOR function.
</details>

<details>
<summary>9. Describe the steps of forward and backward propagation in Neural Networks.</summary>

Answer: 
1. Guess some value for coefficients.
2. Compute the direction of the gradient.
3. Move some distance in that direction.
</details>

<details>
<summary>10. What is the problem of vanishing gradient?</summary>

Answer: Large changes in input result in very small changes in the derivative. This problem is compounded as multiple small gradients are multiplied in hidden layers.
</details>

<details>
<summary>11. How can the vanishing gradient problem be addressed?</summary>

Answer: 
1. Normalize inputs.
2. Use other activation functions.
</details>

<details>
<summary>12. How is the number of parameters in a Neural Network determined?</summary>

Answer: # parameters = #weights + #biases
</details>

<details>
<summary>13. If one node is added to a Neural Network, how will the number of parameters change?</summary>

Answer: The change in the number of parameters would depend on the architecture of the network and where the node is added. Generally, it would increase by the number of connections the node has (weights) plus one (for the bias).
</details>

<details>
<summary>14. Why is the sigmoid function important in logistic regression?</summary>

Answer: The sigmoid function is used to squash the output between 0 and 1, making it useful for binary classification tasks in logistic regression.
</details>

<details>
<summary>15. What is the role of the non-linear transformation in a Neural Network Unit?</summary>

Answer: The non-linear transformation introduces non-linearity to the model, allowing it to capture more complex relationships in the data.
</details>

<details>
<summary>16. Why are Neural Networks considered to be more versatile than traditional regression models?</summary>

Answer: Because of their ability to model complex non-linear relationships through multiple layers and units.
</details>

<details>
<summary>17. What is a computation graph's significance in understanding neural network operations?</summary>

Answer: It helps visualize the operations and their sequence, providing a clearer picture of the data flow and computations in the network.
</details>

<details>
<summary>18. How is the XOR problem addressed in Neural Networks?</summary>

Answer: The XOR problem is addressed using multiple layers in the neural network with specific weight and bias configurations to model the non-linear XOR relationship.
</details>

<details>
<summary>19. Why does the vanishing gradient problem pose challenges for training deep neural networks?</summary>

Answer: It makes the weights of the initial layers (closer to the input) change very little, preventing the model from learning effectively and can lead to slower convergence.
</details>

<details>   
<summary>20. What are the potential advantages of normalizing inputs in Neural Networks?</summary>

Answer: Normalizing inputs can help in faster convergence, prevent the model from getting stuck in local minima, and can mitigate the vanishing/exploding gradient problems.
</details>

# Model Complexity
<details>
<summary>1. What does the phrase "There is no free lunch in Statistics" imply?</summary>
It implies that there is no single method that dominates others in statistics.
</details>

<details>
<summary>2. In the context of regression setting, what is the goal in terms of MSE?</summary>
We want a model that minimises the MSE on test data, not just the training data.
</details>

<details>
<summary>3. How might the training MSE and test MSE differ?</summary>
A method with the lowest training MSE may not necessarily have the lowest test MSE.
</details>

<details>
<summary>4. What is the Bias-Variance trade off?</summary>
It's the balance between how well a model can approximate the true structure (bias) and the amount by which the model would change if training data was changed (variance).
</details>

<details>
<summary>5. What does irreducible error represent?</summary>
The amount by which the model's predictions would change if the training data was changed. If variance is high, small changes in training data result in large changes in the model.
</details>

<details>
<summary>6. What happens if the true model is non-linear and we use linear regression?</summary>
The linear regression will have a high bias.
</details>

<details>
<summary>7. In the context of Bias-Variance trade off, what do flexible methods tend to have?</summary>
Flexible methods have high variance.
</details>

<details>
<summary>8. What is the significance of the vertical dotted line in the example provided?</summary>
The vertical dotted line indicates the flexibility level corresponding to the smallest test MSE.
</details>

<details>
<summary>9. How is Explainable AI (XAI) described in "Weapons of Math Destruction" by Cathy O’Neil?</summary>
It is described as “highly efficient, seemingly arbitrary, and utterly unaccountable … no one will understand their logic or be able to explain it.”
</details>

<details>
<summary>10. Why is it important for users to understand explanations in XAI?</summary>
So that they have a clear understanding of which variables or feature interactions impacted model predictions, and they can discern the model's strengths and weaknesses.
</details>

<details>
<summary>11. What should XAI processes provide insights about?</summary>
XAI processes should shed light on the ways in which outcomes will be used by an organization.
</details>

<details>
<summary>12. In terms of MSE, what is the primary difference between training data and test data?</summary>
The MSE is computed using the training data, but in general, we are interested in the accuracy of the model on unseen test data.
</details>

<details>
<summary>13. How are the true function and its estimates visually represented in the given lecture?</summary>
The true function (f) is shown in black while three estimates of f are shown: the linear regression line (orange curve), and two smoothing spline fits (blue and green curves).
</details>

<details>
<summary>14. What is the relationship between squared bias, variance, and test MSE as shown in the examples?</summary>
The examples show squared bias (blue curve), variance (orange curve), Var(ε) (dashed line), and test MSE (red curve) for three different data sets.
</details>

<details>
<summary>15. Why is explainability important in AI?</summary>
Explainability facilitates an understanding of the variables or features that impact model predictions, provides insights into a model's strengths and weaknesses, and ensures users understand the explanations.
</details>

# Applications
<details>
<summary>1. How do investments benefit from satellite-image analysis?</summary>
Satellite-image car counting or tracking of shipping containers provides an informational advantage that yields 4% to 5% in the three days around quarterly earnings announcements.
</details>

<details>
<summary>2. What is the potential risk of using voice recognition for identification?</summary>
There's a risk that generative AI could be trained to fool the voice recognition AI, leading to potential false identifications.
</details>

<details>
<summary>3. How is NLP beneficial for financial analysis?</summary>
NLP can be used to extract information and relations from textual data such as using tweets to predict stock sentiment, analysis for financial statements, and ESG analysis of firms.
</details>

<details>
<summary>4. What is the primary use of ML in asset pricing or portfolio construction?</summary>
Machine Learning can be used to identify factors that yield better portfolio construction.
</details>