# k-Nearest Neighbors (k-NN) Classifier

This Python script implements a k-Nearest Neighbors (k-NN) classifier, which is a simple but effective supervised machine learning algorithm for classification. The k-NN algorithm classifies data points based on the majority class of their k-nearest neighbors in a labeled dataset. It can be used for a variety of classification tasks.

## Prerequisites

Before running the script, make sure you have the following libraries installed:

- [NumPy]
- [Pandas]: For data manipulation.
- [argparse] For command-line arguments.


## Usage

To run the script, use the following command:

```bash
python knn_classifier.py --data data_file.csv --k 3
```

- `data_file.csv`: The path to the CSV file containing your dataset. The CSV file should have columns for data points, and each point should have an 'x' and 'y' value. The 'label' column is used for classification.
- `k`: The value of k for the k-NN classifier, which determines the number of nearest neighbors to consider.

## Algorithm

The script implements the k-NN classification algorithm with the following steps:

1. Read the dataset from the specified CSV file.
2. Initialize the initial case base (`IB2`) with the first data point.
3. Update the case base and dataset by comparing each data point with the existing case base.
4. Calculate the distances between data points and neighbors in the case base.
5. Determine the k-nearest neighbors for each data point.
6. Assign the majority class label among the k-nearest neighbors as the predicted label.
7. Count classification errors and print the error count.

The script will count and print the classification errors and display the final labels assigned to the data points.
