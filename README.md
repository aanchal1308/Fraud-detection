# Credit card fraud detection
Machine learning algorithm to detect fraudulent credit card transactions.

#### Dataset
The dataset of of nearly 28,500 credit card transactions was used to identify transactions with a high probability of being credit card fraud.
The dataset can be downloaded from [kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)

### Outlier-Detection Algorithms
The following two machine learning algorithms are deployed for outlier detection.

**Local Outlier Factor (LOF)**
The anomaly score of each sample is called Local Outlier Factor. It measures the local deviation of density of a given sample with respect to its neighbors. It is local in that the anomaly score depends on how isolated the object is with respect to the surrounding neighborhood.

**Isolation Forest Algorithm**
The IsolationForest ‘isolates’ observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature.
Since recursive partitioning can be represented by a tree structure, the number of splittings required to isolate a sample is equivalent to the path length from the root node to the terminating node.
This path length, averaged over a forest of such random trees, is a measure of normality and our decision function.
Random partitioning produces noticeably shorter paths for anomalies. Hence, when a forest of random trees collectively produce shorter path lengths for particular samples, they are highly likely to be anomalies.

### Run
To run this python code on your machine, run 'jupyter notebook credit-card-fraud.ipynb' in terminal or command prompt.
This will open the project in Jupyter notebook
