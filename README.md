# hieroglyph_recognizer

You can download the pretrained VGG-19 models weights from : https://www.kaggle.com/keras/vgg19

After that , VGG-19.ipynb notebook creates the full model from those weights and saves it as a full model.

Then, we use the VGG-19 models first 4 layers as our siameese network.

After making that model predict our images, we get two matrices. After we calculate the distance between these two matrices, we get a variable that contains the difference of two images' features.

Then, we feed that output to a regular fully connected network to create an binary classification task.


This model is created to compare an image with all images in the dataset and if it is similar to one of them, return its label.

This model is still under construction.


Note to Myself : You may use cosine similarity instead of difference in the siameese model next time.
