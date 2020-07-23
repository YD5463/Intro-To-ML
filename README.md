# Vision & Hand State Detection

This project came to summarize the concepts we learn over this semester.

- Unsupervised Machine learning models
- Model Based on Boosting technique
- Dimensionality reduction technique
- Pandas version 1.0



## Part A:

In this part we take the Fashion Mnist dataset and use dimensionality reduction techniques like PCA and SVD

to extract the most importance features(from 784 to 23).

After that we use model based boosting and other basic models.

Also, we use in unsupervised model like k means and "translate" the clustering to our labels(types of clothes)

Note: As A bonus we use conventional neural network

### **Scores Summery**:



##### Using machine learning regular model:



|      model name       | score without PCA | score with PCA |
| :-------------------: | :---------------: | :------------: |
| Naive Bayes(Gaussian) |        58%        |      74%       |
|  K Nearest Neighbors  |        86%        |                |
|     Decision Tree     |        81%        |      76%       |
|          SVC          |        87%        |      89%       |
| K Means(unsupervised) |        78%        |      78%       |



##### Using ensemble learning:



|          model name          | score without PCA | score with PCA |
| :--------------------------: | :---------------: | :------------: |
|        Random Forest         |        88%        |      86%       |
| Adaptive Boosting (adaboost) |        82%        |      78%       |
|           XgBoost            |        90%        |                |



##### Using deep learning:



|          model name           | score |
| :---------------------------: | :---: |
|  neural network(Sequential)   |  84%  |
| Sequential with layers change |  90%  |





## Part B:

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



### The Results



| Model Name            | Validation Score |      |
| --------------------- | ---------------- | ---- |
| K Nearest Neighbors   | 88%              |      |
| Sequential Neural Net | 79%              |      |
| XgBoost               | 72%              |      |
| Adaptive Boosting     |                  |      |
| Random Forest         | 95%              |      |
|                       |                  |      |

