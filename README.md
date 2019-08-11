# Active Learning For Integrating Sparse Datasets: A Comparison of Different Query Strategies and Learning Algorithms

Data matching is the task of identifying and matching records from different datasets that refer to the same real world entity. One of the fundamental issues in data matching is creating a training dataset where pairs in the dataset are assigned a label representing their match status. This often involves highly time consuming manual labeling. In order to overcome this, active learning algorithms can be used where the algorithm chooses the instances it wants to learn from and therefore reaches the same accuracy while using significantly less amount of data. In the thesis active learning has been applied to match products collected from different websites against a manually prepared product catalog. This task involves certain challenges which haven't been addressed widely in the literature that includes; finding appropriate strategies to handle missing values prior to data matching, trying different query strategies for data matching tasks and employing different learning algorithms in combination with active learning strategies. 

Our approach to this task includes proposing and using two new strategies to handle missing values in data matching, calculating similarities between records using levenstein, jaro-winkler and jaccard similarity metrics, using active learning strategies of uncertainity, query by committee, density weighted and random sampling for querying instances in combination with support vector machine, logistic regression, decision tree and random forest machine learning algorithms. Additionally a variation of batch active learning has been used for active learning and feature selection with F Classification has also been embedded into the active learning algorithm. The results of the applied algorithms have been analyzed from the aspect of accuracy measured by f1 score, convergence and time. As a result of the thesis, it has been found out that uncertainitiy sampling that uses random forest, jaccard similarity calculated features and handles missing values by adding new columns to the feature vector while assigning 1 if either of the fields under comparison is missing. The model has an average F1 score of 0.8, reaches convergence after 13 iterations and training time of 29 minutes, overall datasets. The codes used in the thesis can be found in github.com/bngksgl/Master\_Thesis. 
