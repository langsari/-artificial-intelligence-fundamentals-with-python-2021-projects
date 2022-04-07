# IMAGE SEGMENTATION USING K-MEAN
## Introduction :
Image Segmentation : In computer vision, image segmentation is the process of partitioning an image into multiple segments. The goal of segmenting an image is to change the representation of an image into something that is more meaningful and easier to analyze. It is usually used for locating objects and creating boundaries. For example, if we seek to find if there is a thing or person inside an indoor image, we may need image segmentation to separate objects and analyze each object individually to check what it is.

It is not a great idea to process an entire image because many parts in an image may not contain any useful information. Therefore, by segmenting the image, we can make use of only the important segments for processing. 

Many kinds of research have been done in the area of image segmentation using clustering. There are different methods and one of the most popular methods is K-Means clustering algorithm.

![image](https://user-images.githubusercontent.com/95903407/162152939-a4ce8f2f-ccbc-432c-9962-8272d91c6ee5.png)

### Working of Image Segmentation :
Image Segmentation involves converting an image into a collection of regions of pixels that are represented by a mask or a labeled image. In image segmentation, pixels which have similar attributes are grouped together. you can process only the important segments of the image instead of processing the entire image.

### Types of Image Segmentation :
Our project is Semantic Segmentation, it is the process of segmenting the image pixels into their respective classes. For example, in the figure below, the cat is associated with yellow color; hence all the pixels related to the cat are colored yellow. Multiple objects of the same class are considered as a single entity and hence represented with the same color.

![image](https://user-images.githubusercontent.com/95903407/162181156-72ae5d5e-b42d-4396-9c90-f9889653cf91.png)

## Problem Statement :
Many parts in some image may not contain any useful information that we wish.  Therefore, the goal of Image segmentation is to change the representation of an image into something that is more meaningful and easier to analyze.

## Requirements :
- Jupyter Notebook

## Importing the Libraries :
- Matplotlib
- SkLearn
- Numpy
- Cv2

## K-Means clustering :
K-Means clustering algorithm is an unsupervised algorithm and it is used to segment the interest area from the background. It clusters, or partitions the given data into K-clusters or parts based on the K-centroids.

The algorithm is used when you have unlabeled data(i.e. data without defined categories or groups). The goal is to find certain groups based on some kind of similarity in the data with the number of groups represented by K.

![image](https://user-images.githubusercontent.com/95903407/162170882-febd6dd1-3775-4e98-b69f-3a34046d6b0d.png)

The objective of K-Means clustering is to minimize the sum of squared distances between all points and the cluster center.

![image](https://user-images.githubusercontent.com/95903407/162153620-eefe6532-7b33-489c-9c5a-02c04aa96261.png)

## Algorithm :
### => Steps in K-Means algorithm :-

1. Choose the number of clusters K.
  
2. Select at random K points, the centroids(not necessarily from your dataset).
  
3. Assign each data point to the closest centroid → that forms K clusters.
  
4. Compute and place the new centroid of each cluster.
  
5. Reassign each data point to the new closest centroid. If any reassignment . took place, go to step 4, otherwise, the model is ready.

### => Steps to choose the optimal number of clusters K (Elbow Method) :- 

1. Compute K-Means clustering for different values of K by varying K from 1 to 10 clusters.
  
2. For each K, calculate the total within-cluster sum of square (WCSS).
  
3. Plot the curve of WCSS vs the number of clusters K.
  
4. The location of a bend (knee) in the plot is generally considered as an indicator of the appropriate number of clusters.    

## Conclusion :
