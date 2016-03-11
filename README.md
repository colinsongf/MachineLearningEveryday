##2016 阅读记录

- 2016-03-05

Xgboost中两个我之前没有用过的特性，一个是[用户自定义代价函数](https://github.com/dmlc/xgboost/blob/master/demo/guide-python/custom_objective.py)，另一个是[pred_leaf](https://github.com/dmlc/xgboost/blob/master/demo/guide-python/predict_leaf_indices.py),预测的时候设置pred_leaf为True，将对每个样本返回其在每棵树上的leaf index（一共有num_round棵树），可以当成新的特征来用。


- 2016-03-07

阅读了[《A Programmer's Guide to Data Mining》](http://guidetodatamining.com/)这本电子书，内容过于简单，两三个小时读完，干货不多。

- 2016-03-08

[Converting categorical data into numbers with Pandas and Scikit-learn](http://fastml.com/converting-categorical-data-into-numbers-with-pandas-and-scikit-learn/)  这篇文章讲了类别特征的处理，文中提到一点需要引起思考：If you have missing values in a binary feature, there’s an alternative representation:-1 for negatives，0 for missing values，1 for positives。It worked better in case of the Analytics Edge competition: an SVM trained on one-hot encoded data with d indicators scored 0.768 in terms of AUC, while the alternative representation yielded 0.778.

- 2016-03-11

[Imbalanced data – Finding Waldo](http://www.financealleycat.com/?p=69)  这篇文章讲了不平衡数据的处理，都是常见的方法（简单采样，合成采样），但是文章最后讲了一个很有趣的处理方式：如果不平衡数据中某个类别的数据非常少，那么也可以把分类问题当成异常值检测的问题（ [anomaly detection](https://en.wikipedia.org/wiki/Anomaly_detection)），只需要检测出异常值就行了。
