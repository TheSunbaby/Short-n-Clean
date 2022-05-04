M E 369P - Team 4 - Short n' Clean 
Allen Hewson, Brenda Miltos, Marcie Legarde, Pranay Srivastava

This repository includes all of the files needed to produce a dataset to train a model to allow a user to play a game of rock paper scissors with a computer. The game includes an easy and a hard mode, where easy bases the computer hand off of random choice, and hard gets the computer to cheat.

Files
1) gather_data.py
    This file captures image data for use in training a model to recognize a hand playing rock paper scissors
    Note: you will have to adjust the file paths to a location in your local directory
2) edge_detection.py
    This file uses the images collected from gather_data.py and prepares new images to train the model using edge detection 
3) EdgeDetectionModelTraining.ipynb - Google Colab. You can use it here: 
    This file trains a model based on the images produced from edge_detection.py
    Note: the file path must match the file path you generated in your local directory
4) recognize_edge.py
    This file is used to test the model generated by EdgeDetectionModelTraining.ipynb.
5) RPSEnv.py
    This file is used to generate an environment for reinforcement learning.
6) main.py
    This file connects the backend for the model and reinforcement learning to the GUI for a game of rock paper scissors (Cow, Snake, Bird)
7) Rock_Paper_Scissors folder
    This folder contains files ready to play a game of rock paper scissors
    Note: the model for these files is not as good as the model set up for Cow Snake Bird