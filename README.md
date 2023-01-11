# Tom-and-Jerry-Image-Classification
Tom and Jerry dataset(https://www.kaggle.com/datasets/balabaskar/tom-and-jerry-image-classification) contains 5478 images extracted from some of Tom & Jerry's show videos, that are available online. The downloaded videos were converted into images with 1 frame per second and labelled manually.

Initially used traditional machine learning approaches like the Stochastic Gradient Descent, Logistic Regression, and Random Forests. As aspected the results were not that good, i.e., accuracy of 0.57 for Stochastic Gradient descent, 0.66 for Logistic Regression, and 0.78 for Random Forests were obtained. 

Then implemented Multilayer perceptron model with accuracy of 0.60 which is much lower than that of the Random Forests classifier. Since the size of the dataset was small (5478 total images), it could be that the Random forests yielded better results. 

Finally, implemented a CNN after resizing and normalising the dataset. Used a sequential model with a rescaling layer, followed by 3 repeating - Conv2D and Maxpooling2D layers with Relu activation, then flattened and finally 2 Dense layers. The trained model performed with an accuracy of 0.852 on test data. But data augmentation did not significantly help cause probably cause the images were already heavily resized to lower size by 10 times.
