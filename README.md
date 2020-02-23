# Predict-target-class-using-KNN

Sometimes we are just given a classified data set where hidden the feature column names are hidden but have given the data and the target classes.

Here, We use KNN to create a model that directly predicts a class for a new data point based on the features.

The data is explored visually using **seaborn** by plotting all the variables against each other using pairplot with value colors defined by the column **'TARGET CLASS'** to check the impact on it with each changing parameter.

The variables are **standardised** with a scale because the KNN classifier predicts the class of a given test observation by identifying the observations that are nearest to it. Any variables that are on a large scale will have a much larger effect on the distance between the observations, and hence on the KNN classifier, than variables that are on a small scale.

A K Nearest Neighbour classifier model is created initially taking neighbours=1 and then predictions are made for the test data.
Then the best value of K is chosen using the **elbow method**.

Then the model performance is evaluated by calculating the Classification Report and Confusion matrix for some suitable K values observed.

To conclude, the KNN classifier model performs well i.e. *approx. 84% accuracy*. We were able to squeeze *approx. 10-12% more*  accuracy out of our model by tuning to a better K value than what was with *K=1*.
