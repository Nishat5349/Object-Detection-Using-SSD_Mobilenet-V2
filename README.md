# Object-Detection-Using-SSD_Mobilenet-V2
It is the extension of my previous Thermal Image-based object detection project. Here, I trained my model using SSD Mobilenet V2 which is a popular deep learning technique.

Transfer learning technique was used for training our model using a MobileNetV2 of the Keras applications module with pre-trained weights using data from the ImageNet dataset.
As a feature extractor, the pre-trained MobileNetV2 model is employed. Then, the MobileNetV2 features are sent through a series of fully connected layers to perform classification on our dataset. With a dropout layer, fully connected layers with ReLU activation and L2 regularization, and a final fully connected layer with softmax activation and L2 regularization, the fully connected layers are defined using the functional API of Keras. The top layers of the MobileNetV2 model are made non-trainable, and only the new fully connected layers are trainable. Then, we used a batch size of 16 and a total of 10 epochs to train our model. Then, using the categorical "cross-entropy" loss function, we constructed the model. For optimizing the model we used "Adam" optimizer.

For our dataset, we get 73% accuracy. The classification report is given below:

![image](https://github.com/Nishat5349/Object-Detection-Using-SSD_Mobilenet-V2/assets/72455268/dd056ba3-8d45-4423-93ca-b5bbf805f95f)

OUR DATASET WILL BE UPLOADED SOON...
