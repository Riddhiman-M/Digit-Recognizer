# Digit-Recognizer
Recognizes digits from pictures of handwritten numbers using the MNIST dataset
<hr>
The train and test data from the MNIST dataset are fetched. The train data has the dimensions (60000, 28, 28) which means, there are 60000 training images of 28x28 pixels each, for example:
<img src="https://machinelearningmastery.com/wp-content/uploads/2019/02/Plot-of-a-Subset-of-Images-from-the-MNIST-Dataset.png" width=40% height=40%>
<br>
Using this train data, we make predictions of the labels of the test data (test images, also of 28x28 pixels).

| Model | Accuracy (in %) |
| :---: | :---: |
| Random Forest Classifier | 96.91 |
| K-Nearest Neighbors | 96.94 |
| Deep Learning Based | 97.75 |
<br>

## Tuning the hyperparameters:<br>
<li> For the K-nearest neighbour model, maximum accuracy was obseved at number of neighbors = 7</li><br> 
<li>For the Deep learning model, a neural network of 2 hidden layers was created each using the <i>ReLU</i> activation function followed by an output layer using the <i>Softmax</i> activation function. An output vector of probabilities was obtained, denoting resemblance with each digit, out of which the maximum one was considered.</li>
