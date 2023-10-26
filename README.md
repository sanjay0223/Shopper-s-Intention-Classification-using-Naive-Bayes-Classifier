# Shopper-s-Intention-Classification-using-Naive-Bayes-Classifier
Utilized Naive Bayes Classifier
Naive Bayes classifiers are a family of simple "probabilistic classifiers" based on applying Bayes' theorem.

It follows strong (naïve) independence assumptions between the features.

Pros: The advantages of using Naive Bayes are as follows:

Easy and fast to predict class of test data set.

Performs well in case of multi-class prediction.

Performs well in case of categorical features as compared to numerical features.

For numerical variable, normal distribution is assumed (bell curve), which is a strong assumption.

When assumption of independence holds, it performs better as compared to other models.

Cons: The disadvantages of using Naive Bayes are as follows: Zero Frequency Problem: In case, if categorical variable has a category in test data set, which was not observed in training data set, then model will assign a zero probability and will be unable to make a prediction.

Solution: Smoothing techniques such as Laplace estimation. Bad estimator: Probability outputs from predict_proba are not to be taken too seriously.

Assumption of Independent Predictors: In real life, it is almost impossible to get a set of predictors which are completely independent.

Before diving further let's get to know some important concepts that are realted to Naive Bayes.


**Insights**:
The classification report  shows the precision, recall, and F1-score for two classes (0 and 1) for both the training and testing datasets. Here's a more detailed interpretation of the metrics:

**Training Set Metrics:**
- For class 0: 
  - Precision: 0.95
  - Recall: 0.68
  - F1-score: 0.79
- For class 1:
  - Precision: 0.32
  - Recall: 0.81
  - F1-score: 0.46
- Accuracy: 0.70

**Testing Set Metrics:**
- For class 0:
  - Precision: 0.96
  - Recall: 0.69
  - F1-score: 0.80
- For class 1:
  - Precision: 0.32
  - Recall: 0.83
  - F1-score: 0.46
- Accuracy: 0.71

 Interpretation:

- **Class 0 (likely the negative class):**
  - The model has a high precision for class 0, meaning when it predicts class 0, it's correct almost all the time.
  - The recall for class 0 is relatively lower, indicating that the model doesn't capture all actual instances of class 0.
  - The F1-score is reasonably high, showing a good balance between precision and recall for class 0.

- **Class 1 (likely the positive class):**
  - The precision for class 1 is low, suggesting that when the model predicts class 1, it often makes false-positive predictions.
  - The recall for class 1 is higher, indicating that the model is better at identifying actual instances of class 1.
  - The F1-score for class 1 is low, suggesting an imbalance between precision and recall.

- **Overall:**
  - The model's accuracy is relatively high for both the training and testing datasets, indicating that it makes correct predictions more often than not.

The conclusion from these metrics depends on the specific requirements of your problem and your priorities regarding precision and recall. Here are some considerations:

- If you need to be very certain that the positive class predictions are accurate (low false positives), you might need to improve the precision for class 1.

- If you want to capture a higher proportion of actual positive instances (high recall), the model already performs well in this regard.

- It's important to consider the trade-off between precision and recall based on the practical implications of false positives and false negatives in your application.

- The F1-score is a good summary metric when you need to balance precision and recall.
