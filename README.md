## MNIST Handwritten Digit Recognition 

For this project I used TensorFlow with Keras to create a convolutional neural network and predict handwritten digits from the well known MNIST dataset. In addition, I used Matplotlib visualization, NumPy for matrix/tensor operations, and scikit-learn for evaluating model accuracy.  

I started by loading the data using TensorFlow and scaled the training and test data. I used Matplotlib to plot a few of the digits in the test dataset to see what it looked like. I started with a simple model using Dense layers but found that it was overfitting. To help with this I decreased model complexity, added dropout layers, and experimented with the learning rate, batch size, and number of epochs. I finally fit the model on all the training data, evaluated with the test data, used scikit-learn to visualize the confusion matrix, and found it has near 97.5% accuracy which is decent, but I could do better. 

Next, I developed a convolutional model. I used 2D convolution and max pooling layers in conjunction with a few Dense layers. Similarly to the last model I added a dropout layer, but I also found using a batch normalization layer worked well for the model. I again evaluated the model accuracy and looked at the confusion matrix. This model was able to reach an accuracy near 99%. I also visualized a few of the images the model got wrong and saw that these digits often had poor legibility which would make sense. 

Finally, I drew one of each digit myself to see if the model could predict them. The model was able to predict each of them which I displayed at the end. 
