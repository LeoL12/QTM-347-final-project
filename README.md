Introduction:
What is the problem:
The problem is to effectively distinguish different geographical features
This dataset comprises images of various scenes, it should be specifically focus on the satellite images
Some landmarks contain various features
Why it is interesting:
The implication of the dataset includes environmental monitoring, urban planning, and virtual reality. 
Successfully addressing this challenge can enhance automated systems' ability to interpret and organize visual data, thereby contributing to advancements in artificial intelligence and machine learning.
Also, satellite model auto-classification can be used in map making, geographical recognition, or military usage
What Approaches?
Convolutional Neural Networks
Data cleaning
CNN includes four layers: 
Convolutional Layers: Feature extraction using filters to detect patterns like edges, shapes, and textures.
Max-Pooling Layers: Downsampling feature maps to reduce computational cost and focus on dominant patterns.
Flatten Layer: Converts the 2D feature maps into a 1D vector to feed into the dense layers.
Fully Connected Layers (Dense Layers): One hidden layer with 128 neurons to learn high-level representations.
Setup:
Used data is from Kaggle
“This dataset contains satellite images of 21 classes such as buildings, baseball fields, freeways, etc. The original size of the images is 256x256 pixels. Originally there were 100 images per class. After augmenting each image 4 times the size of each class was brought up to 500 images.”
Total images: 10,000.
Number of classes: 20.
Image resolution: Varies, but all images are resized to 150×150 times pixels for training.
Result:
The CNN achieved a test accuracy of 85%, demonstrating strong performance on the given dataset. Validation accuracy closely tracked training accuracy, indicating that the model effectively generalizes without significant overfitting.
Data augmentation improved generalization by introducing randomness to the training data.
A learning rate of 0.001 provided stable convergence during training.
Batch size of 32 was optimal for balancing memory usage and training speed. 
Training loss decreased steadily over 20 epochs, while validation loss plateaued, showing the model converged effectively.
Discussion:
Dataset Size: The dataset may not represent real-world variability
Hyperparameter Sensitivity: The results could vary with different learning rates or batch sizes, requiring careful tuning.
Alternative Models: Pre-trained deep networks may achieve higher accuracy but at the cost of increased computational resources.
Conclusion:
The model achieved a high accuracy
It takes too long to run which failed the convenience purpose
Require a specific type of image
Probably not appeal to popular needs




