# MNIST_PCA_KNN
This repository contains a script that demonstrates the use of Principal Component Analysis (PCA) and k-Nearest Neighbors (kNN) for the task of handwritten digit recognition using the MNIST dataset.

## Understanding PCA and kNN
Principal Component Analysis (PCA)
PCA is a statistical technique used for dimensionality reduction. It transforms the data into a new coordinate system, reducing the number of variables while preserving as much variance as possible. This is particularly useful for large datasets like MNIST, as it simplifies the data without losing significant information, thus making subsequent analysis more efficient.

## k-Nearest Neighbors (kNN)
kNN is a simple, non-parametric, and lazy learning algorithm used for classification and regression. It classifies a data point based on how its neighbors are classified. In this project, kNN is used to classify the MNIST digits into their respective categories after the dimensionality reduction by PCA.

## Project Description
The PCA_KNN.py script performs the following steps:

- Load and Preprocess Data: The MNIST dataset is loaded, and the data is separated into features and labels.
- Apply PCA: PCA is used to reduce the dimensionality of the dataset, retaining the components that explain a significant amount of variance.
- kNN Classification: The kNN algorithm is applied to the reduced data for digit classification.
- Performance Evaluation: The classification accuracy is computed to evaluate the performance of the model.

## Insights and Observations
### Results
The PCA-kNN model achieved an accuracy of 97% on the MNIST test dataset and 85% on the MNST fashion dataset.
The PCA step significantly reduced the computation time for the kNN algorithm without a substantial drop in accuracy.

### Learnings
- Effectiveness of PCA: This project highlighted the effectiveness of PCA in reducing dataset complexity, making it easier for algorithms like kNN to process high-dimensional data.
- Balancing Accuracy and Efficiency: The project showcased the trade-off between accuracy and computational efficiency. Reducing dimensions too much can lead to loss of important information, while too few reductions might not simplify the task sufficiently.

### Comparison with Other Techniques
Compared to more complex models like neural networks, the PCA-kNN approach is simpler and faster, though it might not capture complex patterns as effectively.
This approach is particularly useful for applications where interpretability and computational efficiency are more critical than achieving the highest possible accuracy.
