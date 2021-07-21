# Speech-Emotion-Recognition
Using the Crema Dataset 2 models were implemented.
One that uses a Conv1D neural network that learns on time domain features extracted from the wav files in the dataset, These features were (Zero crossing rate & root mean square value)
The other model uses a Conv2D neural network that leans on a Mel-Spectrogram that is treated as an image and is processed as an image.
The dataset was split into 70% train set and 30% test set, Where the train set is split into 5% of the train set to be validation set when training the neural network.
Feautre extraction was done by Librosa and The model was impletented by Tensorflow 2.0 and Keras.

The Conv1D model did an accuracy of 49% on a test set.
With the Conv2D 3 models with similar arhitectures were implemented, the 3 models gave accuracies between 60% ~ 61.8%
Using the 3 Conv2D models a simple ensemble was created that worked with max voting on the test set. Using the Ensemble an accuracy of 64% on the test set was achieved.
