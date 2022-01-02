# *An introduction to data science project*

##### *Student name*: Yosef Danan

## *Part 1:*

this part discuss about plots in matplotlib and seaborn libraries.

the dataset contains information about apps in apple store and our task was to visualize the data
(so we can learn more about the data)

## *Part 2:*

this part discuss about run supervised learning algorithm from scikit-learn library on one dataset from Kaggle, I choose google play apps dataset and my goal was to predict whether or not apps will success, my definition to "success" app was above 1M installs, and to make it more interesting I also defined something in the middle called "good" app that was above 200k.<br>

my features to predict was:<br>

- **size** in megabytes of the app<br>
- **Type** that tells if app is paid or free(0 or 1)<br>
- general **Category** of the app(between 0 to 12)<br>
- **Content Rating** that tells the audience that fit to the app(teen, everyone etc.)<br>

and choose to ignore the **Rating** and **Reviews** features because we know at the end(when we also know the installs numbers).<br>

just to remind **The null hypothesis** was that all 3 states of success(great , good and failed) distribute uniformly namely that non of the features above not influencing the success state<br>

Part of my models shows good result:<br>

- **K-Nearest Neighbors** with 92% accuracy score and the value of K didn't make much of an impact<br>

- **Decision Tree** with 88% accuracy score (after k fold cross validation method, with 5 folds)<br>

- **Random Forest** with 88% accuracy score<br>

- **Gaussian Naive Bayes** with 84% accuracy score<br>

- **Support vector machines** with 91% accuracy score<br>

- **Adaptive Boosting** with 90% accuracy score<br>

  part of them shows really **bad result:**

- **Logistic Regression** with 26% accuracy score<br>

- **Neural Network** with 39% accuracy score<br>

***In conclusion:***  the most of the mistakes of the successful models was in classify between class 1(good app) and 2(successful  app).<br>

