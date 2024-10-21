# Deep Learning Project: Sentiment Analysis on IMDB reviews using Long short-term memory (LSTM)

## Table of Contents
- [Project Overview](#project-overview)
- [Objective](#objective)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Dependencies and Installation](#dependencies-and-installation)
- [How to Run](#how-to-run)
- [Results](#results)
- [Future Work](#future-work)
- [References](#references)

## Project Overview
This project aims to build a deep learning model using Long Short-Term Memory (LSTM) to predict the sentiment of movie reviews based on the IMDB 50K dataset. By leveraging the strengths of LSTMs in processing sequential data, the model analyzes text reviews to classify them as positive or negative.

## Objective
The primary objective of this project is to accurately classify movie reviews into binary sentiments (positive or negative) by utilizing deep learning techniques, specifically LSTM networks.

## Dataset
The dataset used for this project is the IMDB dataset available on Kaggle. You can find the zip file in the `datasets` folder. Here is the link to the dataset: [IMDB Dataset on Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews). This dataset is designed for binary sentiment classification and contains substantially more data than previous benchmark datasets. It provides a set of 25,000 highly polar movie reviews for training and another 25,000 for testing.

## Model Architecture
The LSTM model architecture consists of an input layer that processes sequences of length 200, followed by an embedding layer that converts input integers into dense vectors of size 128. The core of the model features an LSTM layer with 128 units, which captures long-term dependencies in the text. To mitigate overfitting, dropout regularization is applied with a rate of 0.2 for both the LSTM layer and its recurrent connections. The model concludes with a dense layer featuring a single neuron and a sigmoid activation function, outputting a probability score to classify the sentiment of the movie review as positive or negative.

## Dependencies and Installation
All the dependencies required for this project can be found in the `requirements.txt` file. Make sure you have Python installed in your environment.

## How to Run 
To set up the environment and run the project, follow these steps:

1. Install the dependencies:
   ```bash
   pip install -r requirements.txt
2. Run the Jupyter notebook to execute the code.

## Results
After training the model, the following results were achieved:
- Test Loss: 0.3078
- Test Accuracy: 87.59%

Every modification or optimization to improve the model is welcome!