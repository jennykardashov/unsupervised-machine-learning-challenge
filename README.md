# unsupervised-machine-learning-challenge

You are on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. Your team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, your supervisor has asked you to explore this possibility by using unsupervised learning.

You have been provided with raw data, so you’ll first need to process it to fit the machine learning models. You will use several clustering algorithms to explore whether the patients can be placed into distinct groups. Then, you’ll create a visualization to share your findings with your team and other key stakeholders.

## Part 1: Prepare the Data

- Data is prepared and dataframe is created using the csv file

- Removed the "MYOPIC" column from the dataset.

## Part 2: Apply Dimensionality Reduction

- Performed dimensionality reduction with PCA.The number of featured reduced to 10 from 14 as the n_components was set to 0.90.

- Further reduced the dataset dimensions with t-SNE and visually inspected the results. To do this, ran the t-SNE on the principal components, which is the output of the PCA transformation.

- Scatter plot is created

## Part 3: Perform a Cluster Analysis with K-means

- Elbow plot is created to find the best number of clusters

- Used a for loop to determine the inertia for each k between 1 through 10.

- Determined the elbow of the plot and the K value.

Part 4: Make a Recommendation

- Using PCA(n_components=0.90) creates a model that will preserve approximately 90% of the explained variance, that means reducing the dataset to 10 principal components
- Using t-SNE,the principal components is further reduced to 2 components to visualize the data.
- From the elbow curve,the inflection point where the slope takes a sharp turn and flattens out is 3.So the optimal number of clusters is 3.
- Using k-means the data is grouped into 3 clusters
