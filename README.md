# SVD_on_MNIST
Imported the dataset from _tensorflow.keras.datasets_ and stored it in a dictionary with the lables as keys and the coresponding images as matrices.
The columns of the matrices are the single images with all 784 pixels.


I used first 3000 images for training and the rest for testing.

First the 4 left singular values of each digits were extracted. Then we used this for the purpose of classification.

Now, using the rank-4 approximation matrix, I computed the projection of each datapoints onto the column space of each lables. The labels for which the residue was minimum was predicted as the actual class for that datapoint.
