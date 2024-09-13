# Neural-Network-Assignment-ICP_4

NAME: RAMA KRISHNA GANTA ID#: 700759560

VIDEO: https: https://drive.google.com/file/d/14r5qEwzSx4kSmd55HmsLchmuvC-GKEkP/view?usp=sharing

1.Use the use case in the class: 
![image](https://github.com/user-attachments/assets/55da4d2f-ac3d-4681-9f52-e25eed4f122f)


1.1 a. Add more Dense layers to the existing code and check how the accuracy changes.
![image](https://github.com/user-attachments/assets/b5486828-8b59-46fd-9947-c30a914834c7)

1.2 Change the data source to Breast Cancer dataset * available in the source code folder and make required changes. Report accuracy of the model. Then we have added the breast cancer dataset then extracting features and labelsthen encoding the label then splitting the data into training and testing dataset and then evaluting the data set.
![image](https://github.com/user-attachments/assets/1a396e7c-ee9f-47fa-862e-fef569584841)

1.3 Normalize the data before feeding the data to the model and check how the normalization change your
accuracy (code given below).
from sklearn.preprocessing import StandardScaler
sc = StandardScaler()

![image](https://github.com/user-attachments/assets/6b8eaf65-7d34-46cc-bf96-2e90c0da3f03)

2.Use Image Classification on the hand written digits data set (mnist)

![image](https://github.com/user-attachments/assets/106f8d09-0bfa-4a9d-b4aa-e6664ee95812)


2.1. Plot the loss and accuracy for both training data and validation data using the history object in the source
code.
![download](https://github.com/user-attachments/assets/ea0042a0-d717-4451-88bb-fd5e9376955e)

![download](https://github.com/user-attachments/assets/77601238-1988-437d-8b02-23f939697501)

2.2. Plot one of the images in the test data, and then do inferencing to check what is the prediction of the model
on that single image.
![download](https://github.com/user-attachments/assets/1a102738-56c2-4ed2-ae44-e0a2edd209ed)


2.3. We had used 2 hidden layers and Relu activation. Try to change the number of hidden layer and the
activation to tanh or sigmoid and see what happens.
![image](https://github.com/user-attachments/assets/499f45dc-c54f-4312-8ed9-70d56ca0161f)

2.4. Run the same code without scaling the images and check the performance?
![image](https://github.com/user-attachments/assets/66781d54-99d5-440c-b730-2ae233458358)
![download](https://github.com/user-attachments/assets/e28ef9ff-00d7-4ed4-87dc-bbcb5f5b8fac)

