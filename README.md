The repository "DLAssignment2" comprises two main parts:

Part A: Focuses on training a Convolutional Neural Network (CNN) from scratch using the Pytorch framework.

Part B: Focuses on fine-tuning parameters of a pre-existing model using Pytorch.

Each part consists of implementation code and testing code, along with sweep configurations. Here's an overview of each part and its components:

Part A:

final_code_partA.ipynb: Contains the implementation of training a CNN in Pytorch. It includes sweep features such as filter shape, L2 regularization, dropout rate, learning rate, activation function, batch size, batch normalization, filter organization, and data augmentation.
Includes code for testing, visualization, and guided backpropagation. It presents the best hyperparameters selected by the sweep, including filter shape, L2 regularization, dropout rate, learning rate, activation function, batch size, batch normalization, filter organization, data augmentation, and number of neurons in the dense layer.
guided_backprop_output.pdf: Displays guided backpropagation applied to CONV5, visualizing the neuron excitation of 10 neurons in that layer under each image.



Part B:

final_code_partB.ipynb: Implements the fine-tuning of a pre-trained model in Pytorch. It includes sweep features such as freezing layers until before the last kth layer, dropout rate, batch size, and number of neurons in the dense layer.
 Contains code for testing on the iNaturalist dataset, showcasing the best hyperparameters, including frozen layers, dropout rate, batch size, and number of neurons in the dense layer.
Sweep Configurations:

Method: Bayes
Metric: Validation accuracy (to be maximized)
Stopping Parameters: Early terminate (type: hyperband, min_iter = 3, s = 2)
Parameters: Mentioned hyperparameters such as filter shape, L2 regularization, dropout rate, learning rate, activation function, batch size, batch normalization, filter organization, data augmentation, number of neurons in the dense layer, and frozen layers.
