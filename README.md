# Generate-TV-Scripts

This project uses a recurrent neural network (RNN) to generate new TV scripts in the style of Seinfeld. The model is trained on part of the Seinfeld dataset of scripts from 9 seasons.

## Data

The training data is in the file ./data/Seinfeld_Scripts.txt. This raw text file contains scripts from 9 seasons of Seinfeld episodes.

## Model

The model is an RNN with LSTM cells. It takes in words encoded as integers and predicts the next word. The neural network is trained with stochastic gradient descent.

## Usage

To generate a new TV script, run the Jupyter notebook dlnd_tv_script_generation.ipynb. The notebook will walk through the following steps:

- Loading and exploring the Seinfeld dataset
- Preprocessing the text data
- Creating vocab to int and int to vocab lookups
- Initializing the RNN model
- Training the model
- Generating a new script by seeding the network with a starting word
- Generated scripts will be printed in the notebook and can also be saved to text files.

## Requirements

The notebook requires the following Python libraries:

- numpy
- torch
- helper functions from helper.py

The notebook was developed with Python 3.6 and PyTorch 0.4.0.

## References

The dataset is from https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv

