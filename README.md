# Epicore_sweat_patch_project
Google Colab files:
Sweat profiling_training model_v2: ResNet50 model used for training 770 images (modified and added more images as per the feedback from Prof. Eni)
Sweat profiling_training model_v1: ResNet50 model used for training 705 images
Two different regression models are trained using the pre-trained ResNet50 neural network architecture using Keras, for the two labels, i.e. Sweat rate and sodium level. The image files are  named as “actual sweat rate_actual sodium level_serialno.jpg”. Hence, the training data labels are extracted from the file names for training the model. The train-test split is 0.15, batch size is 1 and the model is trained for 12 epochs. The mean absolute error is computed at every iteration. Once the model is trained the labels for the test samples are predicted and the R^2 is computed at each iteration. A plot to show the actual and predicted values is displayed to get an intuition about the closeness of the true and predicted labels.

Jupyter notebooks:
Template Matching: Contains code for template matching using a template image. The same code was modified and the parameters were tuned for preprocessing all the training images. A sample test image is used for demonstration.
Sweat_rate: Code for extraction of orange channel and computing the area of that contour in terms of number of pixels. Again, the same code was used for all the training images with different threshold values (fine tuning-based on different images)
Electrolyte_level: Code for extraction of purple channel and reference swatches, computing their RGB values and plotting the calibration curves for the four NaCl experiments. All the training images were labelled using the same code with adjustments in the threshold values for finding the RGB values.

The result images for the template matching are also included in the same folder. The code is commented to understand the algorithm.                    

