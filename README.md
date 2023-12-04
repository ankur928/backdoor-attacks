# Neural Network Backdoor Detection Using Channel Pruning

## Details
Name: Ankur Aggarwal  
Net ID: aa10336

## Table of Contents
1. [Overview](#overview)
2. [System Requirements](#system-requirements)
3. [Repository Structure](#repository-structure)
4. [Installation and Operation Guide](#installation-and-operation-guide)
5. [Data](#data)
6. [Directory Structure](#directory-structure)
7. [Contributions](#contributions)
8. [Acknowledgements](#acknowledgements)

## Overview
This repository hosts the code for a novel neural network backdoor detection system. The project's goal is to enhance security in neural networks, particularly BadNets trained on the YouTube Face dataset, by developing an advanced model named GoodNet. GoodNet is engineered to differentiate between normal and compromised (backdoored) inputs, classifying them into separate categories.

## System Requirements
Execution Environment: MacBook Pro equipped with M1 chip
Interface: Jupyter Notebook

## Repository Structure
Notebook_PruneDefense.ipynb: Core Jupyter Notebook with pruning defense logic and GoodNet construction.
model_evaluation.py: Script to assess model accuracy on untainted and compromised datasets.
Dataset/: Folder containing valid.h5 for validation and test.h5 for testing.
Saved_Models/: Storage for original, modified, and GoodNet models.

## Installation and Operation Guide
Download the repository to your system.
Set up a compatible Jupyter Notebook environment, ideally on a MacBook Pro with an M1 chip or an equivalent setup. Executing this project on Google colab is not recommended as it is very slow.
Install all required dependencies listed in requirements.txt.
Confirm the Dataset/ folder has the necessary data files.
Launch Notebook_PruneDefense.ipynb in Jupyter Notebook and run the cells in order.
For model evaluation, run model_evaluation.py, adjusting paths as needed for your environment.

## Data
1.  Download the validation and test datasets from  [here](https://drive.google.com/drive/folders/1Rs68uH8Xqa4j6UxG53wzD0uyI8347dSq?usp=sharing) and store them under  `lab4/data/`  directory.
2.  The dataset contains images from the YouTube Aligned Face Dataset. We retrieved 1283 individuals and split them into validation and test datasets.
3.  bd_valid.h5 and bd_test.h5 contains validation and test images with sunglasses trigger respectively, that activates the backdoor for bd_net.h5.

## Directory Structure
The project is organized as follows:

- `data/`: Contains datasets for validation and testing.
  - `cl/`: Clean datasets.
    - `valid.h5`: Clean validation data for defense design.
    - `test.h5`: Clean test data for BadNet evaluation.
  - `bd/`: Datasets with sunglasses-poisoned images.
    - `bd_valid.h5`: Validation data with backdoor trigger.
    - `bd_test.h5`: Test data with backdoor trigger.
- `models/`: Houses the neural network models.
  - `bd_net.h5`: The backdoored neural network model.
  - `bd_weights.h5`: Weight parameters for the model.
- `architecture.py`: Defines the neural network architecture.
- `eval.py`: Script for evaluating the model's performance.

## Contributions
Feedback and contributions are highly encouraged. For proposing changes or discussing new ideas, please initiate an issue or submit a pull request.

## Acknowledgements
Appreciation goes to the team behind CSAW-HackML-2020 for their foundational work and dataset provision.
Acknowledgement of NYU's support and resources in facilitating this research.
