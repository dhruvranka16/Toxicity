# Toxicity
This repository contains a machine learning model and dataset for detecting toxicity in text comments. The model is built using TensorFlow and utilizes a Bidirectional LSTM neural network.

Dataset
The dataset used in this project consists of text comments and labels indicating the presence of toxicity in the comments. The labels are binary, with 1 indicating toxicity and 0 indicating non-toxicity. The dataset is split into a training set, a validation set, and a test set.

Model Architecture
The toxicity detection model is built using the following layers:

Text Vectorization Layer: The text data is preprocessed using the TextVectorization layer from TensorFlow. It tokenizes the text and converts it into integer sequences.

Embedding Layer: An embedding layer is used to convert the integer sequences into dense vectors. It has a vocabulary size of 200,001 and an embedding dimension of 32.

Bidirectional LSTM Layer: This layer contains a Bidirectional LSTM (Long Short-Term Memory) network with 32 units and a tanh activation function. It helps capture contextual information in the text data.

Fully Connected Layers: After the LSTM layer, there are three fully connected layers with ReLU activation functions. These layers serve as feature extractors.

Output Layer: The final output layer consists of 6 units with a sigmoid activation function. It provides binary predictions for each toxicity category.

Training and Evaluation
The model is trained for one epoch using the training dataset and evaluated on the validation dataset. The model's performance metrics, such as precision, recall, and accuracy, are calculated and reported.

Usage
Prerequisites
Before using the model, make sure you have the following libraries and dependencies installed:

TensorFlow
Pandas
NumPy
Matplotlib
