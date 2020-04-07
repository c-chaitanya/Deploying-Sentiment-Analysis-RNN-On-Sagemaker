# SageMaker Deployment Project

The notebook and Python files provided here, result in a simple web app which interacts with a deployed recurrent neural network performing sentiment analysis on movie reviews. This project uses python3.6, basic html and SageMaker for deployment.

# Deploying a Sentiment Analysis Model

## Project Overview

In this project, I have used Amazon SageMaker to complete an entire lifecycle of a machine learning project. The goal is to build a very simple web page in which a user can submit a movie review and the prediction model behind the scenes will predict whether it is Positive or Negative review. The prediction model is implemented using Pytorch framework and trainned on IMDB dataset.


## Project Instruction

This entire project is done on Amazon sagemaker and uses some heavy GPU instances for training the models. If you want execute this on local machine, you might want to train the model on subset of the training data from IMDB dataset. Also there are steps where we upload the data to amazon S3 instances in order to train using aws instances which you can totally ignore on local machines

### Instructions to execute in sagemaker

1. Clone the repository on your sagemaker notebook instance.
	```
	https://github.com/c-chaitanya/Deploying-Sentiment-Analysis-RNN-On-Sagemaker.git
	```
2. Run the `SageMaker Project.ipynb` file using.
	```
	jupyter notebook SageMaker Project.ipynb
	```
3. Read and follow the instructions! You can find and download the dataset for this project in the notebook.


### General Outline

- Step 1: Downloading the data
- Step 2: Preparing and Processing the data
- Step 3: Upload the data to S3
- Step 4: Build and Train the PyTorch Model
- Step 5: Testing the Model
- Step 6: Deploying the model for testing
- Step 7: Use the model for testing
- Step 6  Deploy the model for the web app
- Step 7  Use the model for the web app

### Libraries

The list below represents main libraries and its objects
for the project.
- [Amazon SageMaker](https://ap-northeast-2.console.aws.amazon.com/sagemaker/home?region=ap-northeast-2#/landing) (Build, train, and deploy a model)
- [tensorflow](https://www.tensorflow.org/) (LSTM classifier)

### Shutdown/Remove These chargable instances post running
### 1) Notebook instance
### 2) Endpoint
### 3) API gateway
### 4) Lambda function
### 5) Data in S3(optional) 
