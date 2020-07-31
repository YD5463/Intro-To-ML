# Vision & Hand State Detection

This project came to summarize the concepts we learn over this semester.

- Unsupervised Machine learning models
- Model Based on Boosting and Bagging technique
- Dimensionality reduction technique
- Pandas version 1.0



## *Part A:*

In this part we take the Fashion Mnist dataset and use dimensionality reduction techniques like PCA and SVD

to extract the most importance features(from 784 to 23).

After that we use model based boosting and other basic models.

Also, we use in unsupervised model like k means and "translate" the clustering to our labels(types of clothes)

Note: As A bonus we use conventional neural network

### **Scores Summery**:



##### *Using machine learning regular model:*



|      model name       | score without PCA | score with PCA |
| :-------------------: | :---------------: | :------------: |
| Naive Bayes(Gaussian) |        58%        |      74%       |
|  K Nearest Neighbors  |        86%        |                |
|     Decision Tree     |        81%        |      76%       |
|          SVC          |        87%        |      89%       |
| K Means(unsupervised) |        78%        |      78%       |



##### *Using ensemble learning:*



|          model name          | score without PCA | score with PCA |
| :--------------------------: | :---------------: | :------------: |
|        Random Forest         |        88%        |      86%       |
| Adaptive Boosting (adaboost) |        82%        |      78%       |
|           XgBoost            |        90%        |                |



##### *Using deep learning:*



|          model name           | score |
| :---------------------------: | :---: |
|  neural network(Sequential)   |  84%  |
| Sequential with layers change |  90%  |





## *Part B:*

In this part we have dataset with hands motion sensor recording we our task is to classify the type of the hands moving:

1. **Spontaneous** 
2. **Synchronized**
3. **Alone**



The features we get from the sensor is:

- Time
- Frame ID 
- Hand Type
- number of hands
- Position(X,Y,Z)
- Velocity(X,Y,Z)
- Pitch
- Roll
- Yaw
- Wrist Position(X,Y,Z)
- Elbow Position(X,Y,Z)
- Grab Strength
- Grab Angle
- Pinch Strength

**Note**: In very record we **ignore** the first 7 seconds. **Also**, we **combine** every 5 rows into 1.



### *The Results*



| Model Name            | Validation Score |
| --------------------- | ---------------- |
| K Nearest Neighbors   | 88%              |
| Sequential Neural Net | 79%              |
| XgBoost               | 100%             |
| Adaptive Boosting     | 99%              |
| Random Forest         | 95%              |
| Decision Tree         | 94%              |



## Sources

- [Intro to data science - washington university](https://www.youtube.com/playlist?list=PLMrJAkhIeNNQV7wi9r7Kut8liLFMWQOXn) - svd part
- [Intro to Machine Learning - fastai](https://www.youtube.com/watch?v=CzdWqFTmn0Y&list=PLfYUBJiXbdtSyktd8A_x0JNd6lxDcZE96) - parts
- [Relationship between svd and pca](https://stats.stackexchange.com/questions/134282/relationship-between-svd-and-pca-how-to-use-svd-to-perform-pca) 
- [Why xgboost so good](https://medium.com/analytics-vidhya/what-makes-xgboost-so-extreme-e1544a4433bb)
- [Ensemble methods](https://towardsdatascience.com/ensemble-methods-bagging-boosting-and-stacking-c9214a10a205)
- [ML approaches for time series](https://towardsdatascience.com/ml-approaches-for-time-series-4d44722e48fe)
- [Git](https://missing.csail.mit.edu/2020/version-control/)
- [Fast.ai course - Practical Deep Learning for Coders](https://www.youtube.com/watch?v=Th_ckFbc6bI&list=PLCdvEQLhYkYm1y0Ufn1FvmfL5pDpadkZN)-just the begin
- [Udacity Course](https://classroom.udacity.com/courses/ud262)
- [Gradient Descent](https://www.youtube.com/watch?v=sDv4f4s2SB8)

and other from medium,towards data science...

**By**: *Yosef Danan*

**Really Cool Project!**

