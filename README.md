# Vegetable-and-Fruit-Analysis-using-deep-learning 
Mounting Google Drive: The code starts by mounting your Google Drive to access the dataset stored there.

Data Preparation: The code defines a function called image_processing to create a DataFrame that contains filepaths and corresponding labels for the images. This function is then used to create separate DataFrames for the training, validation, and test sets.

Data Visualization: The code displays a grid of sample images from the training set using matplotlib.

Data Generators: ImageDataGenerator objects are created for the training, validation, and test sets. These generators apply preprocessing functions to the images and provide batches of augmented images during training.

Model Creation: The MobileNetV2 model is loaded with pre-trained weights from the ImageNet dataset. A custom dense layer is added on top of the base model, and the final output layer is configured for multi-class classification.

Model Compilation and Training: The model is compiled with an optimizer, loss function, and evaluation metrics. The fit function is called to train the model using the training and validation data. Early stopping is implemented to prevent overfitting.

Model Evaluation: The trained model is used to predict the labels for the test set. The predictions are converted back to their corresponding class labels using a mapping dictionary.

Prediction Function: The code defines a function called output that takes an image location as input and uses the trained model to predict the label for that image.
