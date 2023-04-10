Designing an unmanned car that can move in the center of the road requires several steps. We will use Python language, OpenCV, NumPy libraries, and neural network along with Linear Regression and Keras library. Here's how to do it:

Step 1: Gathering Data
We need to gather data for our neural network to train on. We will be using the MNIST dataset for handwritten digit recognition and the German Traffic Sign dataset for identifying traffic signs. The MNIST dataset contains 60,000 images for training and 10,000 images for testing, and the German Traffic Sign dataset contains over 50,000 images of different traffic signs.

Step 2: Preprocessing Data
We will be using OpenCV to preprocess our data. For the MNIST dataset, we will resize the images and flatten them into a 1D array. For the German Traffic Sign dataset, we will resize the images to a smaller size and convert them to grayscale.

Step 3: Creating the Neural Network
We will create a Convolutional Neural Network (CNN) using the Keras library. A CNN is especially good at image classification tasks as it can learn hierarchical features of the input data. We will use two convolutional layers followed by two max-pooling layers, followed by a flatten layer and two dense layers. The last dense layer will have 10 units for the MNIST dataset and 43 units for the German Traffic Sign dataset to classify the respective categories.

Step 4: Training the Neural Network
We will train the neural network using the preprocessed datasets. We will use a batch size of 32 and train for 10 epochs.

Step 5: Linear Regression 
For the unmanned car to move in the center of the road, we need to use a linear regression model to calculate the position of the car. We can use our trained CNN to detect the boundaries of the road and create a region of interest. We then use the edges of this region to determine the position of the car relative to the center of the road.

Step 6: Integration
We can now integrate our CNN and linear regression models into the unmanned car. The car will use the CNN to detect the boundaries of the road and create a region of interest. This region will then be used by the linear regression model to calculate the position of the car relative to the center of the road. The car can then be programmed to move towards the center of the road based on this position.

In conclusion, by using Python, OpenCV, NumPy libraries, and neural network along with Linear Regression and Keras library, we can design an unmanned car that moves in the center of the road. This can be achieved by using a CNN to detect the boundaries of the road and a linear regression model to calculate the position of the car relative to the center of the road. The integration of these models will allow the car to move towards the center of the road.