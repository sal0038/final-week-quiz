# Data Science Quiz

### Instructions

- Fork and Clone
- Work on quiz
- Push back up to your repository

### Questions

1. A vector is given, `[2,3,9]`. What's the norm?

- 9.69

2. I have a biased 6-sided die. P(T) = 0.45. What's the probability, if I flip the coin 100 times, that I will get exactly 14 heads?

- 2.89 ^ 11

3. What is the rank of a matrix?

- The maximum number of linearly independent vectors in a matrix

4. Why is rank important for Linear Regression?

- Columns need to be linearly independent to work otherwise coefficeints will not be right

5. What is the purpose of the sigmoid function in a Logistic Regression model?
 - Turns logodds into probabilities. If you add a threshold, will help you make classifier predictions.

6. What is bias vs variance?
 - Bias = Difference between avg. prediction and correct value (the error). Leads to high error.
 - Variance = Spread of data. Good on training data but weak on test data. 

7. What is a hyperparameter? What part of the dataset (train, validation or test) is responsible for determining this value?

 - Setting of a model to reduce the error. Can use for train or validation. For validation, example would be gridsearch b/c iterating through trying to find the best parameter.

8. Model selection via cross validation. What part of the dataset (train, validation or test) is responsible for choosing the best model?

 - Validation

9. What is parametric vs non-parametric model?

- Parametric assumes a distribution for the data i.e (X, SQRT) for normalizing data and non-parametric assumes no distribution
- Parametric models are numerical based (assumes a distribution to the dataset) vs non-parametric models which are based on non-numerical models (no assumptions that they fit to any distribution)

10. What models do you need to scale the data prior to fitting?

- Any models that use Euclidean distances - most of the time, datasets will contain features highly varying in magnitudes, units and range

11. What is entropy? Which model uses this concept?
- Measure of disorder in the dataset. Used for decision trees and random forest. Splliting until lowest entropy.

12. How is a random forest generated?
- A random forest is a collection of decision trees that are split on different features. When the forest makes a prediction it will either take the average or the majority depending on if the model is a regression or classification. This method reduces variance.

13. How do you determine the correct number of clusters when using KMeans?
 - Elbow method - WSS plotted out and where bend indicates number of clusters to use
 - Silhouette method - Optimal K maximizes avg. silhouette score. Silhouette plot shows how close points are in one cluster compared to    another.

14. What is a dendrogram?
 - Visual represenation of hierachical clsutering that show how datapoints are clustered together.

15. What is linkage?
- There are two parts previous to this. Pdist is distance between all points in a vector. Squareform combines these into a square matrix and linkage is used to create clusters from this. Merges two clusters with smallest distance together that are not in the same cluster into one cluster. 

16. How does a recommender model work?
- Recommender models look at rankings by user or rankings by items. It looks for similarities between rankings by user or items and makes a prediction for future users based on similar users or items. Use matrix factorization when need to inpute missing values for users and or items that have not been ranked. 

17. How can you reduce the number of features in a model?
- Feature importance from tree based models , Lasso, correlation and PCA

18. What is a good use of PCA?
 -  PCA is best used for visualization, data clustering, and datacompression. Reduce the number of features in a dataset. Use on dataset that could have multiple linear relationships which could cause colinearity  

19. In general, how do neural networks "learn"?
- Neural networks learn through a process called back propagation. Data is fed through the layers of a network, an output is produced, some type of error calculation is done and the error is fed back to the network. This process continues until the error is kept at a minimum  

20. What is your favorite model? Why?
 - Logistic Regression. Like classification models and somewhat easy to interpret.
