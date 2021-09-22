# Music_genre_Classifier
Musical genres are categorical labels created by humans to characterize 
pieces of music. A musical genre is characterized by the common 
characteristics shared by its members. These characteristics typically are 
related to the instrumentation, rhythmic structure, and harmonic content of 
the music. Genre hierarchies are commonly used to structure the large 
collections of music available on the Web.

We have developed the music genre classification using Convolutional 
Neural Network (CNN), using 3 convolution layers, each with its own max 
pool and Batch Normalization , feeding into 3 fully connected layers with 
ReLU activation, softmax output, and sparse_categorical_crossentropy loss. 
Dropout layer has been implemented in the 3rd convolutional layer after there 
was an overfitting in the training dataset. Dropout works by randomly setting 
the outgoing edges of hidden units (neurons that make up hidden layers) to 0 
at each update of the training phase. We used sparse categorical cross 
entropy because our genre classes are mutually exclusive as we trained the 
model with 400 epochs.

Before we use the dataset we have extract the features from it, so we will 
extractMel-frequency cepstral coefficients also known as MFCC are a feature 
widely used in automatic speech and speaker recognition.
