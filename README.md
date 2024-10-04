# Iris Dataset Clustering with K-Means

This project demonstrates the application of the K-Means clustering algorithm to the famous **Iris flower dataset**. It includes data exploration, visualization, outlier handling, and clustering analysis to find the optimal number of clusters.

## Dataset

The dataset used in this project is the **Iris flower dataset**, which contains 150 samples from each of three species of Iris flowers: *Iris-setosa*, *Iris-versicolor*, and *Iris-virginica*. Each sample includes four features:
- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`

The target variable is the species of the flower, which is not used during clustering but aids in visual analysis.

You can download the dataset from Kaggle:  
[Iris Dataset on Kaggle](https://www.kaggle.com/datasets/arshid/iris-flower-dataset)

You can download My project from Kaggle:  
[My project on Kaggle](https://www.kaggle.com/code/mohamadrezazaheri/k-means-machine-learning-algorithms)


## Project Workflow

1. **Data Loading and Exploration:**
   - The dataset is loaded using `pandas` and basic exploratory analysis is performed, including checking the distribution of each feature.
   
2. **Data Visualization:**
   - The distribution of features across different species is visualized using violin plots, count plots, and pair plots with Seaborn.
   - Boxplots are used for detecting outliers.
   
3. **Outlier Handling:**
   - Outliers in the `sepal_width` feature are identified and replaced using the interquartile range (IQR) method to mitigate their impact.

4. **K-Means Clustering:**
   - K-Means is applied to the dataset, and the optimal number of clusters is determined using the **Elbow Method** by plotting the inertia values for different numbers of clusters.
   - After determining the optimal value of `K=3`, the data is clustered and visualized.

5. **Cluster Visualization:**
   - Scatter plots are used to visualize the clusters along with the centroids.
   
6. **Performance Evaluation:**
   - The **Silhouette Score** is used to evaluate the quality of the clustering.

## Key Results

- The optimal number of clusters is determined to be **3** using the Elbow Method.
- The **Silhouette Score** for the clustering is `0.553`, indicating reasonably well-separated clusters.

## Visualizations

The project includes several visualizations such as:
- **Violin plots** for each feature grouped by species.
- **Pair plots** to show the relationships between all pairs of features.
- **Boxplots** for detecting and handling outliers.
- **Scatter plots** to visualize the clustering results.

## Libraries Used

- `pandas`
- `numpy`
- `seaborn`
- `matplotlib`
- `scikit-learn`

