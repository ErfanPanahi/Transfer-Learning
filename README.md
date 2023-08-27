# Transfer-Learning
In this repository, I intend to implement the idea of Transfer Learning for the EfficientNetB0 network. To achieve this, based on the selected dataset (images of cats and dogs), I will modify the last layer of the EfficientNetB0 network in a way that the network's output will only be the label of either "cat" or "dog."

In this project, we intend to design a network using EfficientNetB0 with the help of a dataset containing two classes, to perform classification between these two classes.

To achieve this, we select a dataset that includes two classes: cats and dogs. Out of a total of 692 images, we consider 400 images as training data, and the rest as testing data.

Dataset Link: https://www.kaggle.com/datasets/samuelcortinhas/cats-and-dogs-image-classification

(Note: The image dog_505.jpg is black and white, not a tensor, so we remove it from the dataset.)

The image below shows the first 10 data points of the training set.

![image](https://github.com/ErfanPanahi/Transfer-Learning/assets/107314081/4f4f31cd-f903-484d-8034-2596bb5f533b)


Now, to create a classifier that distinguishes between these two classes, we first remove the final layer of the EfficientNetB0 network and replace it with a layer with an output size of 2. The reason for having the final output layer with a size of 2 is due to the number of classes in the dataset. The image below displays accuracy and loss values on the training data, and finally, accuracy and the confusion matrix on the test data.

![image](https://github.com/ErfanPanahi/Transfer-Learning/assets/107314081/144ef313-1944-4275-aafb-dabdbb424d5e)

![image](https://github.com/ErfanPanahi/Transfer-Learning/assets/107314081/ea07a758-3c6a-4b50-8052-b0e4f0876dc8)
