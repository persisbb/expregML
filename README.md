
# Here are few insights and learnings from the course and project:
*	Learned about Google Colab and GPUs and How we can utilize these Resources for solving High level Computational Problems where Datasets consist of Images, Text, and Videos.
*	Learned how to build convolutional neural networks on Google Colab and re use the trained objects in our local machine to perform real time predictions.
*	Got introduced to Open CV and Dlib and created a model that can detect different expressions in a face images which are black and white.
*	Performed data augmentation on our images to make our model more robust and efficient.
*	Also performed two phase training on our models, where we have frozen a few layers before our model starts overfitting. 
*	Also evaluated our model on test set and applied real time prediction.

#### Various Approaches to Improve Training: 
* Performing face detection and cropping face images in our training dataset.  Although we have closely cropped faces in our dataset, they are very noisy.   By filtering out all images which were not detected by face detection algorithm we can make our model more robust.
* Increase Number of phases and Decrease number of epochs per phase while training. For example:  You can train a model using a phase 1 with 6 epochs repeated by phase 2 with 4 epochs for 2 times. 
* Try out a better version of EfficientNet. There are even better versions of EfficientNet such as B3 to B7. We have used EfficientNetB2 just to keep it less computationally intensive. So that it can be executed even on Low hardware specification. 
