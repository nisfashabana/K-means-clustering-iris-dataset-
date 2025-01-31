# K-Means-clustering on iris-dataset
## Project Overview

This project applies K-Means Clustering on iris dataset to explore and visualize unsuprevised machine learning techniques.The primary focus is on evaluating clustering performance using the Elbow Method(Distortion) and Silhouette Scores,and interpreting the results to select the optimal number of clusters.

## Dataset

The iris dataset contains 150 observations with the following features:
* sepal_length(cm)
* sepal_width(cm)
* petal_length(cm)
* petal_width(cm)
* species (for validation.though not used in clustering)

## Project Objectives

#### 1.Apply K-Means Clustering to group similar data points.                                                                           
#### 2.Evaluate clustering performance using:                                                                                                         
  * Elbow Method:identifies the point of diminishing returns for clustering inertia.
  * Silhouette Scores:Balances cluster cohesion and seperation.
                                                                                  
#### 3.Visualize the clustering results                                                                                                               
#### 4.Compare and select the best k-value for clustering. 


## Dependencies

Python 3.X
Libraries:

pip install seaborn matplotlib scikit-learn pandas



## Usage Instructions

#### 1.Run clustering Analysi
  Execute the main script to visualize both the Elbow and Silhouette plots:

  python kmeans_iris_analysis.py

#### 2.Key Sections of the Code:

  •Data preprocessing: Standardizes the dataset using StandardScaler.                                                                                                                            
  •K-Means Clustering: Applies clustering for varying  k  values.                                                                                                                                                    
  •Elbow Plot: Visualizes the distortion score (inertia) across different clusters.                                                                                                                                    •Silhouette Plot: Shows silhouette scores for different  k  values.


## Key Outputs

#### 1.Elbow Method:

  Helps determine the optimal  k  by identifying the “elbow” point where distortion reduction slows down.
  
#### 2.Silhouette Plot:

  Suggests the best  k  by indicating how well data points fit within their clusters.
  
#### 3.Cluster Visualization:

  Visualizes clusters formed by K-Means with different  k  values.

## Interpreting the Results

   •The Elbow Method often suggests a smaller  k  for compact clusters, while the Silhouette Score prefers values with better-defined cluster separation.  
   
   •Choose  k  based on both visual inspection and domain knowledge.   
   
   •Example decision:
         •If Elbow suggests  k=4  and Silhouette suggests  k=2 , try evaluating  k=3  as a compromise.

	

## Conclusion

This project demonstrates how to combine clustering metrics like Elbow and Silhouette methods to make informed choices about  k . It highlights the importance of balancing data structure with interpretability.

