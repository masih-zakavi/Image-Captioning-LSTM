### Image Captioning with CNN+RNN model ###
This is a simple image captioning neural network written in TensorFlow. 
It is trained on Flikr30k images that include photos of animals.
The Convolutional Neural Network (CNN) extracts features from the input images
and then a Recurrent Neural Network (RNN) generates captions based on the input.

- To speed-up the training process, the VGG16 model is imported from
TensorFlow with pre-trained weights from ImageNet. Features are extracted
from the input using this CNN. 

- The output of the CNN is then passed to the RNN to generate captions. Since
no weights are imported, the RNN is trained on captions from the dataset. To
make sure long range dependencies are better captured, LSTM is used as the RNN
network.
