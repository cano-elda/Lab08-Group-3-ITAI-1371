Elda's Entry

I learned that making a dataset with a clear pattern and some random noise is a good way to see how different models fit the data.
The graph made it easier for me to notice that even thought the points were spread out, they still followed the general shape of a
sine wave. Comparing polynomial models with degrees 1, 4, and 15 also showed me how a model's complexity can change its predictions.
This lab helped me understand why finding a good balance between bias and variance is important when choosing a model.



Xinyu's Entry:

For this lab, I worked on Task 2 to create learning curves for two polynomial regression models. The first model was of polynomial degree 1, and the other was of degree 15. I used the learning_curve function to get the average training and cross-validation scores for a range of training sizes.

The zero training score for the degree 1 model indicates poor performance of this model. As the number of instances for training is increased, the cross-validation score for this model also increases, and it seems to approach some limit. The model is not able to capture the relevant information in the data set, and so it performs poorly. This is a case of underfitting, which is related to high bias.

For the degree 15 model, the training score was roughly equal to 1.0 for all sample sizes considered, and the corresponding cross-validation score is extremely low (nearly as low as the score for predicting a constant value equal to the average target value). This is because the very complex model has such numerical instability problems that it cannot make accurate predictions for new data. However, for the data given for the problem, the model fits the data for the training set given extremely well (training score roughly equal to 1).

One thing that I learned from this experiment is how one can interpret learning curves. In the past, I only looked at the one score for the model, but learning curves show how one would expect the training and validation scores to change as the number of training examples is increased. For example, a big difference between training and validation scores can indicate overfitting, whereas low scores throughout the learning curve can indicate underfitting. In the experiment above, the scores for the experiments are R² scores. Therefore, R² scores that are less than 0 are worse than predicting the average target value for a data set.
