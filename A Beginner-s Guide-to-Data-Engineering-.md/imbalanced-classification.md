https://www.datasciencecentral.com/profiles/blogs/dealing-with-imbalanced-datasets
Title: Imbalanced big data classification: A distributed implementation of SMOTE
Library: ACM DL Digital Library
Conference: 19th International Conference of Distributed Computing and Networking
Paper URL: https://lnkd.in/fnD6dZE

https://www.analyticsvidhya.com/blog/2016/10/investigation-on-handling-structured-imbalanced-datasets-with-deep-learning/
Q4. You are given a data set on cancer detection. You’ve build a classification model and achieved an accuracy of 96%. 
Why shouldn’t you be happy with your model performance? What can you do about it?

Answer: If you have worked on enough data sets, you should deduce that cancer detection results in imbalanced data. 
In an imbalanced data set, accuracy should not be used as a measure of performance because 96% (as given) might only 
be predicting majority class correctly, but our class of interest is minority class (4%) which is the people who actually
got diagnosed with cancer. Hence, in order to evaluate model performance, we should use Sensitivity (True Positive Rate), 
Specificity (True Negative Rate), F measure to determine class wise performance of the classifier. If the minority class 
performance is found to to be poor, we can undertake the following steps:

We can use undersampling, oversampling or SMOTE to make the data balanced.
We can alter the prediction threshold value by doing probability caliberation and finding a optimal threshold using 
AUC-ROC curve.
We can assign weight to classes such that the minority classes gets larger weight.
We can also use anomaly detection.

https://www.analyticsvidhya.com/blog/2016/03/practical-guide-deal-imbalanced-classification-problems/

sensitivity or true positive rate (TPR)
eqv. with hit rate, recall
TPR = TP/P = TP/(TP+FN)

specificity (SPC) or true negative rate
SPC=TN/N=TN/(TN+FP)

precision or positive predictive value (PPV)
PPV=TP/(TP+FP)

accuracy (ACC)
A
C
C
=
(
T
P
+
T
N
)
/
(
T
P
+
F
P
+
F
N
+
T
N
)
{\mathit {ACC}}=({\mathit {TP}}+{\mathit {TN}})/({\mathit {TP}}+{\mathit {FP}}+{\mathit {FN}}+{\mathit {TN}})
F1 score
is the harmonic mean of precision and sensitivity
F
1
=
2
T
P
/
(
2
T
P
+
F
P
+
F
N
)
{\mathit {F1}}=2{\mathit {TP}}/(2{\mathit {TP}}+{\mathit {FP}}+{\mathit {FN}})