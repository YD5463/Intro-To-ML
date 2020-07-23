# Vision & Hand State Detection





## Part A:



### **scores summery**:



##### using machine learning regular model:



|      model name       | score without PCA | score with PCA |
| :-------------------: | :---------------: | :------------: |
| Naive Bayes(Gaussian) |        58%        |      74%       |
|  K nearest neighbors  |        86%        |                |
|     Decision Tree     |        81%        |      76%       |
|          SVC          |        87%        |      89%       |
| K Means(unsupervised) |        78%        |      78%       |



##### using ensemble learning:



|          model name          | score without PCA | score with PCA |
| :--------------------------: | :---------------: | :------------: |
|        Random Forest         |        88%        |      86%       |
| Adaptive Boosting (adaboost) |        82%        |      78%       |
|           XgBoost            |        90%        |                |



##### using deep learning:



|          model name           | score |
| :---------------------------: | :---: |
|  neural network(Sequential)   |  84%  |
| Sequential with layers change |  90%  |





## Part B: