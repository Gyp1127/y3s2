# Credit Card & Transactions
<details>
<summary>1. What does fraud in the context of credit, debit, or EFTPOS cards involve?</summary>
Fraud involves the use of credit, debit, or EFTPOS card or other details to make purchases or withdraw cash without the account owner's permission. This could include using stolen credit card details. The user can generally recognize a fraudulent transaction with ease, and typically, the financial institution is liable.
</details>

<details>
<summary>2. How does a scam differ from fraud?</summary>
A scam is a fraudulent invitation, request, notification, or offer, designed to obtain personal information or money, or otherwise obtain a financial benefit by deceptive means. Examples include spoofing a website or job scams. Users generally won't recognize a scam until it is too late, and they are typically liable for any losses incurred.
</details>

<details>
<summary>3. How is a credit card technically defined?</summary>
A credit card is technically defined as a revolving line of credit that allows the holder to borrow money or get ‘credit’ from a bank. It is considered debt, with interest chargeable as per the terms of the card, and often has associated fees and other benefits. A credit card does not necessarily have to be a physical card.
</details>

<details>
<summary>4. What are the two types of fraud in credit card transactions?</summary>
The two types of fraud in credit card transactions are:
1. Unauthorized use of an actual physical card (Card present fraud), which can occur if the card is stolen, lost, or not received, or if the card has been counterfeited (e.g., by skimming).
2. Use of card details remotely (Card not present fraud), which can happen due to leaked details from a hack on servers that store card information, phishing details using websites, emails, messages, or through scams.
</details>

<details>
<summary>5. What has been the trend in the relative share of counterfeiting in card fraud?</summary>
Over time, the relative share of counterfeiting in card fraud has reduced.
</details>

<details>
<summary>6. What percentage of card fraud is related to lost or stolen cards?</summary>
The percentage of card fraud related to lost or stolen cards has been more or less stable over time.
</details>

<details>
<summary>7. What is the scale of credit card fraud transactions in the SEPA region for 2021?</summary>
In 2021, there were €1.53 billion in fraud transactions in the SEPA region.
</details>

<details>
<summary>8. How do domestic and cross-border transactions compare in terms of their share of all transactions and fraudulent transactions?</summary>
Domestic transactions accounted for 89% of all transactions and 36% of fraudulent transactions. In contrast, cross-border transactions represented 9% of all transactions and 49% of fraudulent transactions.
</details>

<details>
<summary>9. What percentage of persons in Australia experienced card fraud in 2021-22?</summary>
In Australia, 8.1% of persons (equivalent to 1.7 million individuals) experienced card fraud in the 2021-22 period.
</details>

<details>
<summary>10. How does the occurrence of scams compare to card fraud and identity theft in Australia in 2021-22?</summary>
In Australia in 2021-22, 2.7% of persons (552,000 individuals) experienced a scam, while 0.8% of persons (159,600 individuals) experienced identity theft. This compares to 8.1% of persons who experienced card fraud.
</details>


# Fraud Detection System

<details>
<summary>1. What are the different timeframes in which processes in FDS operate?</summary>
- Real Time
- Near Real Time
- Offline
</details>

<details>
<summary>2. How does a terminal function in the FDS?</summary>
- Responsible for simple mechanical checks
- Very fast to execute
</details>

<details>
<summary>3. What are Transaction blocking rules?</summary>
- Simple “if-then” style rules
- Only current transaction details are considered (does not take into account historical transactions or card holder’s profile).
- Example: If online payment and website is deemed insecure, then deny payment.
- Rules are often manually designed.
- Should have high precision (i.e., raise few false alarms)
</details>

<details>
<summary>4. What checks are performed on authorized transactions after the initial approval?</summary>
- Transaction data compared against historical data and cardholder’s profile.
- Relevant historical data includes average expenditure, average number of transactions, location of transactions etc.
</details>

<details>
<summary>5. What is feature engineering in the context of FDS?</summary>
Computing new transaction properties based on historical data and cardholder’s profile.
</details>

<details>
<summary>6. How are Scoring Rules defined in FDS?</summary>
- Simple “if, then” rules that assign a fraud score to transactions.
- Designed by experts.
- Uses historical information.
</details>

<details>
<summary>7. What is the role of a Data Driven Model in FDS?</summary>
- Purely data driven based on classification models.
- Trained on historical data.
- Generally, the model will output the probability of a transaction being fraudulent.
</details>

<details>
<summary>8. What are the responsibilities of Investigators in FDS?</summary>
- Look at emerging patterns.
- In charge of controlling alerts raised by models.
- Provide feedback to the system.
</details>

<details>
<summary>9. What security concerns arise with the use of phones and smart watches for payments?</summary>
- A token is stored in devices (rather than card details).
- Tokens often have an expiry.
- Vulnerable to theft and “Man in the middle” attacks.
</details>

<details>
<summary>10. How is a transaction labeled as fraudulent in FDS?</summary>
Given a transaction feature vector, a classifier function outputs a probability that denotes the transaction being fraudulent. A threshold is considered, and a transaction will be labeled as fraudulent if the probability is greater than or equal to the threshold.
</details>

<details>
<summary>11. What are the considerations while deciding on the input to the classifier?</summary>
- Should we use real world data or lab data?
- What to include as part of the input to the classifier?
- How do we know that the classifier is “good”?
- What are the challenges in building a good classifier?
</details>

<details>
<summary>12. What challenges are faced in fraud detection?</summary>
- Imbalanced dataset.
- Dataset shift.
- Insufficiency of basic information in a transaction for classification.
- Interpretability.
</details>

<details>
<summary>13. How is Luhn’s algorithm utilized in checking card numbers?</summary>
- Double the value of every other digit.
- Sum the digits from the previous step separately.
- Sum the remaining digits from the card.
- The sum of the two previous steps should be divisible by 10.
</details>

<details>
<summary>14. What kind of rules are designed for the Transaction Blocking Rules?</summary>
Simple “if-then” style rules that often do not consider historical transactions or the card holder’s profile.
</details>

<details>
<summary>15. What is meant by "feature augmentation" in FDS?</summary>
It refers to the process of computing new transaction properties to enhance the dataset, also known as feature engineering.
</details>

<details>
<summary>16. How are scoring rules designed?</summary>
They are "if, then" rules designed by experts using historical information to assign a fraud score to transactions.
</details>

<details>
<summary>17. How is a Data Driven Model in FDS trained?</summary>
It's purely data driven and is trained on historical data.
</details>

<details>
<summary>18. What kind of patterns do Investigators look for in the FDS?</summary>
Emerging patterns that can indicate fraudulent activity.
</details>

<details>
<summary>19. Why are tokens used in devices like phones and smartwatches for payments?</summary>
Tokens are considered more secure than storing actual card details.
</details>

<details>
<summary>20. What is the significance of the threshold in labeling a transaction as fraudulent?</summary>
A transaction is labeled as fraudulent if the output probability from the classifier function is greater than or equal to the set threshold.
</details>

<details>
<summary>21. How does dataset imbalance pose a challenge in fraud detection?</summary>
The number of fraudulent transactions is a tiny fraction compared to genuine transactions, making it difficult for models to accurately detect fraud.
</details>

<details>
<summary>22. Why is dataset shift a concern in fraud detection?</summary>
Fraud tactics evolve over time, making it necessary for models to be regularly updated.
</details>

<details>
<summary>23. Why is interpretability important in FDS?</summary>
Experts should be able to understand why a transaction was labelled as fraudulent to validate the model's decisions and improve its accuracy.
</details>

<details>
<summary>24. What are some of the considerations or questions one should think about when building a classifier for fraud detection?</summary>
- The type of data to use (real world vs. lab data).
- Features to include as input.
- Metrics to evaluate the classifier's performance.
- Challenges in building an effective classifier.
</details>

<details>
<summary>25. How does technology exacerbate fraud challenges?</summary>
The use of devices like phones and smartwatches for payments introduces vulnerabilities like token expiry, theft, and "Man in the middle" attacks.
</details>

<details>
<summary>26. How does the FDS deal with transactions from websites deemed insecure?</summary>
If an online payment is made through a website deemed insecure, the Transaction Blocking Rules can deny the payment.
</details>

<details>
<summary>27. What role does feature engineering play in enhancing fraud detection?</summary>
It involves creating new transaction properties based on historical data and the cardholder’s profile to enhance the dataset, which can improve the accuracy of fraud detection.
</details>

<details>
<summary>28. How do scoring rules in FDS make use of past fraud patterns?</summary>
Scoring rules are often based on past fraud patterns to assign a fraud score to transactions.
</details>

<details>
<summary>29. What is the main goal of a classifier function in FDS?</summary>
To output a probability that indicates whether a given transaction is fraudulent.
</details>

<details>
<summary>30. Why is basic information in a transaction often not sufficient for accurate fraud detection?</summary>
Because fraud tactics are complex and continuously evolving, requiring the need to generate new features and transformations for accurate detection.
</details>


# Synthetic Data & Feature Engineering

<details>
  <summary>1. What is the objective of using synthetic data to build a classifier?</summary>
  
  The objective is to estimate a model such that it is a good approximation of the true model in nature (i.e., the real world).
</details>

<details>
  <summary>2. Why might one construct their own version of truth (�′) when building a classifier?</summary>
  
  The assumption is that if one can estimate �′ well, then they can also estimate the true � well.
</details>

<details>
  <summary>3. What is one advantage of using synthetic data in fraud detection?</summary>
  
  It allows one to control for the types of fraud they are interested to model.
</details>

<details>
  <summary>4. Why would synthetic data be generated to reflect real world transactions?</summary>
  
  To have more confidence in the evaluation of classifiers against modeled fraud scenarios.
</details>

<details>
  <summary>5. What general principles should be followed when generating synthetic data that mimics the true model?</summary>
  
  The data should be highly imbalanced, contain both numerical and categorical features, allow for temporal fraud scenarios, and generate the same challenges as with real world data.
</details>

<details>
  <summary>6. How are customers and terminals represented in the conceptual model?</summary>
  
  Customers and terminals are identified by an ID and are placed on a square grid.
</details>

<details>
  <summary>7. What does the distance between customers and terminals in the conceptual model imply?</summary>
  
  The distance could imply the frequency of shopping, among other things.
</details>

<details>
  <summary>8. What do transaction profiles indicate about the majority of purchases?</summary>
  
  The majority of purchases happen around noon (gaussian distribution) and the majority of the mass is on small value transactions.
</details>

<details>
  <summary>9. What happens when a terminal or card is compromised in terms of fraudulent transactions?</summary>
  
  A compromised terminal or card will have fraudulent transactions for a certain time period.
</details>

<details>
  <summary>10. What are the available features in a given transaction?</summary>
  
  TX_DATETIME, CUSTOMER_ID, TERMINAL_ID, TX_AMOUNT, TX_FRAUD.
</details>

<details>
  <summary>11. Why is the information in a single transaction often not enough to build a good classifier?</summary>
  
  Statistical/Machine learning often requires numerical and ordered features that are relevant to predict the label, and a single transaction might lack some of these.
</details>

<details>
  <summary>12. What is "feature engineering"?</summary>
  
  It is the transformation of existing features and design of new features.
</details>

<details>
  <summary>13. How does binary encoding (one—hot encoding) work?</summary>
  
  It transforms a categorical variable to numerical values, where only one bit is active at a time.
</details>

<details>
  <summary>14. What are the three components of RFM?</summary>
  
  Recency (R), Frequency (F), and Monetary Value (M).
</details>

<details>
  <summary>15. How can the risk of a terminal be evaluated in terms of fraud?</summary>
  
  By building a metric to measure terminal risk based on the number and ratio of fraudulent transactions from that terminal over a certain period.
</details>

<details>
  <summary>16. Why is the status of a transaction not immediately known in practical scenarios?</summary>
  
  Because there might be a delay or it's not straightforward to determine if a transaction is fraudulent or genuine immediately.
</details>

<details>
  <summary>17. In the context of feature engineering, what is risk encoding?</summary>
  
  Risk encoding involves building a metric to measure terminal risk based on the number and ratio of fraudulent transactions from that terminal over a period.
</details>

<details>
  <summary>18. How is a categorical variable transformed into numerical values using binary encoding?</summary>
  
  Through one-hot encoding, where each category is represented by a bit string with only one bit active at a time.
</details>

<details>
  <summary>19. Why might one use synthetic data over real data in fraud detection?</summary>
  
  Synthetic data allows for more control over the types of fraud being modeled and is easier to control for noise.
</details>

<details>
  <summary>20. In the conceptual model, how are transactions generated?</summary>
  
  Transactions are generated based on customer and terminal profiles, including their shopping behavior.
</details>
