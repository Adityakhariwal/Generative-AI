# Problem Statement
With the advent of generative AI, it has become easily difficult to separate real data from AI-Generated.
The goal is to develop a model that can identify a fake photo created by AI.
# Motivation
With the rise of generative AI, fake identities can be easily created using sophisticated algorithms. This has led to an increase in identity fraud, as fake identities can be used to gain access to online services and commit fraudulent activities. Thus, the purpose is to contribute to the development of more secure and reliable online services for everyone.
# Dataset
The Test and Train datasets have been taken from https://bitgrit.net/competition/18 
The training dataset consists of 5250 examples with 1200 columns is used for training different models to identify whether an image is real or fake.
The label for the fake image was 0 and of real image was 1
# Training Using Logistic Regression
![image](https://github.com/Adityakhariwal/Generative-AI/assets/104224483/eb7906e4-2c1e-44eb-a7e1-cde306fc8fd2)


This was not very efficient model and was giving an accuracy of 0.7628571428571429
# Training Using Gradient Boosting
![image](https://github.com/Adityakhariwal/Generative-AI/assets/104224483/81dba78e-b55d-43e0-8a0a-a86981553aff)


setting the values of n estimators = 100, learning rate = 0.1, max depth = 3, random state = 20 , I got the accuracy of 0.8542857142857143
# Training Using CNN
It consists of multiple layers, including convolutional layers, pooling layers, and fully connected layers.
Here we have to adjust the image dimensions according to neural layer size
Batch size was set to 100 , epoches was set to 30 and the model was trained using training dataset which gives the accuracy of 0.8428571224212646 and F1 score of 0.6680080482897384
![image](https://github.com/Adityakhariwal/Generative-AI/assets/104224483/e9940b4f-6a91-411e-a5d7-73a9a36ed86e)

# Training Using ViT
![image](https://github.com/Adityakhariwal/Generative-AI/assets/104224483/f5dc3c03-1868-4438-9d1b-0347357cec99)


Patch size is 5X5 , batch size = 64 , learning rate = 0.0001 gives the average loss of 0.08

ViT took more time to run as compared to any other models for same number of epochs and batch size, but gave more accurate results.

# Results 
F1 score of test data set = 0.69155844 on bitgrit submission
