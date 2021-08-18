# Scaling-and-Transformation-Techniques-Feature-Engineering

* Feature scaling is a method used to normalize the range of independent variables or features of data .Therefore, the range of all features should be normalized so that each feature contributes approximately proportionately to the final distance. 
<hr>

### When We use Feature scaling ? 

* Gradient Descent Based Algorithms
Machine learning algorithms like linear regression, logistic regression, neural  network, etc.If an algorithm uses gradient descent, then the difference in ranges of features will cause different step sizes for each feature. To ensure that the gradient descent moves smoothly towards the minima and that the steps for gradient descent are updated at the same rate for all the features, we scale the data before feeding it to the model. Having features on a similar scale will help the gradient descent converge more quickly towards the minima.

* Distance Based Algorithms :
Distance algorithms like KNN, K-means, and SVM are most affected by the        range of features. This is because behind the scenes they are using distances between data points to determine their similarity.
<hr>

### When scaling your data is NOT necessary?
* Tree-based algorithms
Tree-based algorithms are fairly insensitive to the scale of the features. A decision tree is only splitting a node based on a single feature. The decision tree splits a node on a feature that increases the homogeneity of the node. This split on a feature is not influenced by other features. Hence, there is virtually no effect of the remaining features on the split. This is what makes them invariant to the scale of the features. Some ML algorithms such as Decision trees, Random Forest, AdaBoost, Naïve Bayes, etc.
<hr>

### Types Of Transformation: <br>

>1. Standardization (Standard Scaler) <br>
>2. Scaling to Minimum And Maximum values-(Normalization)-( MinMax Scaler) <br>
>3. Scaling To Median And Quantiles(Robust Scaler) <br>
>4. Guassian Transformations: (When data is not in normal/gaussian distribution) <br>
>   &nbsp;&nbsp;  4(a) Logarithmic Transformation <br>
>   &nbsp;&nbsp;  4(b) Reciprocal Trnasformation <br>
>   &nbsp;&nbsp;  4(c) Square Root Transformation <br>
>   &nbsp;&nbsp;  4(d) Exponential 
