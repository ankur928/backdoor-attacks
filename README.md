# Neural Network Backdoor Detection Using Channel Pruning

## Details
Name: Ankur Aggarwal  
Net ID: aa10336

## Table of Contents
1. [Overview](#overview)
2. [System Requirements](#system-requirements)
3. [Repository Structure](#repository-structure)
4. [Installation and Operation Guide](#installation-and-operation-guide)
5. [Contributions](#contributions)
6. [Acknowledgements](#acknowledgements)

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

## Contributions
Feedback and contributions are highly encouraged. For proposing changes or discussing new ideas, please initiate an issue or submit a pull request.

## Acknowledgements
Appreciation goes to the team behind CSAW-HackML-2020 for their foundational work and dataset provision.
Acknowledgement of NYU's support and resources in facilitating this research.
