# Neural-Network-Assignment-ICP_4

NAME: RAMA KRISHNA GANTA ID#: 700759560

VIDEO: https: https://drive.google.com/file/d/14r5qEwzSx4kSmd55HmsLchmuvC-GKEkP/view?usp=sharing

1.Use the use case in the class: 
![image](https://github.com/user-attachments/assets/55da4d2f-ac3d-4681-9f52-e25eed4f122f)


1.1 a. Add more Dense layers to the existing code and check how the accuracy changes.

Solution:

It starts with a dense layer of 20 neurons and a ReLU activation function. Two additional hidden layers are added, one with 10 neurons and the other with 5 neurons, both using ReLU activation. The final output layer consists of 1 neuron with a sigmoid activation function, suitable for binary classification tasks. The model is compiled using the Adam optimizer and binary crossentropy loss function, and its accuracy is evaluated. By modifying the number of layers and neurons, you can observe how the model's accuracy changes.

![image](https://github.com/user-attachments/assets/b5486828-8b59-46fd-9947-c30a914834c7)

1.2 Change the data source to Breast Cancer dataset * available in the source code folder and make required changes. Report accuracy of the model. Then we have added the breast cancer dataset then extracting features and labelsthen encoding the label then splitting the data into training and testing dataset and then evaluting the data set.

Solution:

This code modifies a neural network model to use the Breast Cancer dataset for binary classification. The dataset is loaded from the provided CSV file, and features (columns 2 to 32) and labels (column 1) are extracted. Labels are encoded using LabelEncoder. After splitting the data into training and testing sets, a sequential neural network model is built with one hidden layer of 20 neurons and an output layer with a sigmoid activation function. The model is compiled using binary crossentropy loss and Adam optimizer. Training is performed over 100 epochs, and the test accuracy is reported to evaluate model performance.

![image](https://github.com/user-attachments/assets/1a396e7c-ee9f-47fa-862e-fef569584841)

1.3 Normalize the data before feeding the data to the model and check how the normalization change your
accuracy (code given below).
from sklearn.preprocessing import StandardScaler
sc = StandardScaler()

Solution:

This code uses the Breast Cancer dataset to build a neural network model, adding normalization to improve performance. After loading the dataset, features are scaled using StandardScaler to normalize the data. Labels are encoded using LabelEncoder. The data is split into training and testing sets, and the neural network is defined with one hidden layer of 20 neurons and a sigmoid output layer for binary classification. The model is compiled with binary crossentropy loss and Adam optimizer. After training the model for 100 epochs, the accuracy is evaluated on the normalized test set to observe the impact of normalization.

![image](https://github.com/user-attachments/assets/6b8eaf65-7d34-46cc-bf96-2e90c0da3f03)

2.Use Image Classification on the hand written digits data set (mnist)

![image](https://github.com/user-attachments/assets/106f8d09-0bfa-4a9d-b4aa-e6664ee95812)


2.1. Plot the loss and accuracy for both training data and validation data using the history object in the source
code.

Solution:

This code adds functionality to visualize the model's performance by plotting training and validation accuracy and loss over epochs using the history object. After training the neural network, the history.history dictionary is used to retrieve accuracy and loss metrics for both training and validation data. Separate plots are generated for accuracy and loss, showing how the model performs over each epoch. The plots provide a visual comparison between training and validation results, helping to assess model generalization and detect potential overfitting.

![download](https://github.com/user-attachments/assets/ea0042a0-d717-4451-88bb-fd5e9376955e)

![download](https://github.com/user-attachments/assets/77601238-1988-437d-8b02-23f939697501)

2.2. Plot one of the images in the test data, and then do inferencing to check what is the prediction of the model
on that single image.

Solution:

This code demonstrates how to plot and infer a prediction on a single image from the test data using a trained neural network model. First, it selects and visualizes one test image using matplotlib's imshow, reshaping the image to its original dimensions (28x28 pixels for this example). Then, the code uses the trained model to make a prediction on the same image and prints the predicted outcome. This process allows verification of the model's performance on individual test samples and can be useful for understanding model predictions in a real-world scenario.

![download](https://github.com/user-attachments/assets/1a102738-56c2-4ed2-ae44-e0a2edd209ed)


2.3. We had used 2 hidden layers and Relu activation. Try to change the number of hidden layer and the
activation to tanh or sigmoid and see what happens.

Solution:

This code modifies the neural network architecture by increasing the number of hidden layers and changing the activation function to tanh for the hidden layers and sigmoid for the output layer. The model is designed with four hidden layers of varying sizes and is compiled using the RMSProp optimizer and categorical crossentropy loss for multi-class classification. The model is trained over 15 epochs, and the performance is evaluated on the test data. By adjusting the number of layers and activation functions, the code helps analyze how these changes impact model accuracy and performance during training and evaluation.

![image](https://github.com/user-attachments/assets/499f45dc-c54f-4312-8ed9-70d56ca0161f)

2.4. Run the same code without scaling the images and check the performance?

Solution:

This code evaluates a neural network on the MNIST dataset without scaling the image pixel values. The MNIST images are reshaped into 1D arrays, but unlike typical preprocessing steps, the pixel values are not scaled (i.e., they remain in the range [0, 255] instead of being normalized to [0, 1]). The model is built with two hidden layers using ReLU activation and a softmax output layer for multi-class classification. It is trained and evaluated without normalization, and the loss and accuracy are plotted for both training and validation data. This approach helps assess how the lack of scaling affects model performance.

![image](https://github.com/user-attachments/assets/66781d54-99d5-440c-b730-2ae233458358)
![download](https://github.com/user-attachments/assets/e28ef9ff-00d7-4ed4-87dc-bbcb5f5b8fac)

