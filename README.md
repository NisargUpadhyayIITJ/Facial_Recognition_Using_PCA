# Facial Recognition Using PCA

This project demonstrates face recognition using Principal Component Analysis (PCA) for dimensionality reduction and a Support Vector Machine (SVM) for classification. The project utilizes the Labeled Faces in the Wild (LFW) dataset.

## Implementation Steps:

Data Loading: The LFW dataset is loaded using sklearn.datasets.fetch_lfw_people. Images with a minimum of 80 faces per person are selected for better recognition accuracy.

Data Splitting: The data is split into training and testing sets using sklearn.model_selection.train_test_split with an 80/20 ratio.

## Custom PCA:

A custom PCA class is implemented to understand the underlying principles of PCA.

The fit method performs data standardization and eigendecomposition of the covariance matrix. 

The transform method projects the data onto the selected principal components.

Dimensionality Reduction: The custom PCA is applied to the training and testing sets, reducing the dimensionality of the data to 100 components.

SVM Training: An SVM classifier is trained using the reduced-dimensionality training data.

Prediction and Evaluation: The trained SVM is used to predict the labels of the test set. The performance is evaluated using a classification report and a confusion matrix.

## Visualization:

A gallery of test images is plotted with predicted and true labels to visually assess the model's performance.

The eigenfaces (principal components) are reshaped and visualized to understand the features captured by PCA.

## Dependencies:

scikit-learn
matplotlib
seaborn
numpy

## Running the Project:

Ensure you have the required libraries installed.

Analyze the classification report, confusion matrix, and visualization plots to understand the model's performance.
