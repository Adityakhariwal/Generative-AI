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
![image](https://github.com/Adityakhariwal/Generative-AI/assets/104224483/47d8f017-eaef-4a0d-b53b-a9fe28e1f7d7)

This was not very efficient model and was giving an accuracy of 0.7628571428571429
# Training Using Gradient Boosting
![image](https://github.com/Adityakhariwal/Generative-AI/assets/104224483/785ce479-403b-4a64-a6b6-f524e528745d)

setting the values of n estimators = 100, learning rate = 0.1, max depth = 3, random state = 20 , I got the accuracy of 0.8542857142857143
# Training Using CNN

