# Flower-Image-Classifier

This project is from my homework for STAT5242 Advanced Machine Learning. <br>
The task is to use a small collection of photos (500 to be exact) to construct a flower-image classifier capable of discerning differences between daisies, roses, dandelions, sunflowers, and tulips.<br>
The dataset is <a href="http://download.tensorflow.org/example_images/flower_photos.tgz">here</a> <br>
The approach is to use transfer learning with the inception network, by leveraging what a pre-trained convolutional neural network has already learned about important image features from the imagenet dataset. Then I removed the last layer, fixed the weights of the remaining layers, used what remains as a black-box function transforming images into derived feature vectors, and finally fitted a new classifier on the derived feature vectors.<br>
transfer_learning.py is an important supplementary module for this task. 
