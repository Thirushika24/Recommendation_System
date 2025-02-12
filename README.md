# Recommendation System

This repository contains implementations of multiple recommendation systems for movies using different approaches and datasets.

## Recommendation Systems Implemented

### Recommendation System 1: Hybrid Model with TensorFlow Recommenders

**Description:** Uses TensorFlow and TensorFlow Recommenders to build a Hybrid Model recommendation system.

**Dataset:** Movielens 100k dataset.

**Features:**

1. Load the MovieLens dataset using tensorflow_datasets.

2. Select relevant features and prepare the vocabulary for user IDs and movie titles.

3. Create UserModel and MovieModel classes to generate embeddings.

4. Define a HybridModel class that uses these embeddings to compute a retrieval task.

5. Train the model on the dataset. Evaluate the model by making recommendations for a sample user and displaying the results.

### Recommendation System 2: Softmax Deep Neural Network Model

**Description:** Implements Softmax Deep Neural Network Model using Keras.

**Dataset:** Movielens 100k dataset.

**Features:**

1. Download and unzip the MovieLens dataset. Merge and refine the dataset to group ratings by user and movie. Encode user IDs and movie titles.

2. Use Keras to define a deep neural network model with user and movie embeddings.

3. Add dense layers with dropout and activation functions to the model.

4. Train the model on the training set and evaluate it on the test set. Plot the training and validation loss over epochs.

5. Make movie recommendations for a sample user based on the trained model.

### Recommendation System 3: K-Nearest Neighbors (KNN) Model

**Description:** Implements K-Nearest Neighbors (KNN) Model for recommendations.

**Dataset:** Movielens 25m dataset.

**Features:**

1. Load the MovieLens dataset. Create a user-item matrix and remove movies with low ratings frequency. Filter active users who have rated more than a threshold number of movies.

2. Use the NearestNeighbors class from sklearn to create a KNN model.

3. Fit the model on the user-item matrix and make movie recommendations for a sample movie.
## Setup and Usage

#### Running the Recommendation Systems:

Each recommendation system is contained in one colab notebook **Movies_Recommendation_System.ipynb**

Open and execute the notebook to explore each recommendation system.

#### Datasets:

The Movielens datasets (ml-100k and ml-25m) are used. You can download them from the Movielens website.

[Dataset](https://grouplens.org/datasets/movielens/)

#### Dependencies:

TensorFlow, TensorFlow Recommenders, TensorFlow Datasets, Scikit-learn, Pandas, NumPy, Keras

## Author

- [@Thirushika S ](https://github.com/Thirushika24/)
