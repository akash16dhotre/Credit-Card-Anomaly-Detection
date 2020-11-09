# Credit-Card-Anomaly-Detection

This is a repository containing a Data Science project called "Credit Card Anomaly Detection". I took the data set from www.kaggle.com and performed Exploratory Data Analysis on the data set. I learned two new Algorithms inorder to successfully complete the project. They are

## Isolation Forest Algorithm :
One of the newest techniques to detect anomalies is called Isolation Forests. The algorithm is based on the fact that anomalies are data points that are few and different. As a result of these properties, abnormalities are susceptible to a mechanism called isolation.

This method is highly useful and is fundamentally different from all existing methods. It introduces isolation as a more effective and efficient means to detect anomalies than the commonly used primary distance and density measures. Moreover, this method is an algorithm with a low linear time complexity and a small memory requirement. It builds a good performing model with a small number of trees using small sub-samples of fixed size, regardless of the size of a data set.

Typical machine learning methods tend to work better when the patterns they try to learn are balanced, meaning the same amount of good and bad behaviors are present in the dataset.

How Isolation Forests Work The Isolation Forest algorithm isolates observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature. The logic argument goes: isolating anomaly observations is more straightforward because only a few conditions are needed to separate those from regular observations. On the other hand, isolating normal observations require more conditions. Therefore, an anomaly score can be calculated as the number of conditions required to separate a given observation.

The way that the algorithm constructs the separation is by first creating isolation trees, or random decision trees. Then, the score is calculated as the path length to isolate the observation.

## Local Outlier Factor(LOF) Algorithm
The LOF algorithm is an unsupervised outlier detection method that computes a given data point's local density deviation with respect to its neighbors. It considers as outlier samples that have a substantially lower density than their neighbors.

The number of neighbors considered, (parameter n_neighbors) is typically chosen:

Greater than the minimum number of objects a cluster has to contain, so that other objects can be local outliers relative to this cluster
Smaller than the maximum number of close by objects that can potentially be local outliers. In practice, such pieces of information are generally not available, and taking n_neighbors=20 appears to work well in general.
