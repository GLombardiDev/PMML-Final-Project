# Probabilistic Methods for Machine Learning - Final Project: Replicating Connect Four AI Agent Moves

This repository contains the report for the final project of the "Probabilistic Methods for Machine Learning" course at the University of Bologna, academic year 2023/24, completed by G. Di Paolo, M. Petracci, and G. Lombardi.  While the code and dataset are not publicly available due to data usage restrictions agreed upon with the providers of the dataset, this report details our approach and findings in replicating the moves of a Connect Four AI agent.

## Project Overview

This project investigated the effectiveness of a Fully Connected Neural Network (FCNN) and a Convolutional Neural Network (CNN) in predicting the moves of an AI agent playing a variant of Connect Four.  We treated the problem as a multi-class classification task, where each class corresponds to one of the seven possible columns for a move.

## Report Highlights

The `report.pdf` document provides a comprehensive overview of our project, including:

* **Problem Definition:** Replicating the move selection strategy of a Connect Four AI agent given a game board state.
* **Methodology:** We developed and trained two deep learning models: an FCNN and a CNN.  Data augmentation was employed by exploiting the game's symmetry.  Hyperparameter tuning was performed using a validation set and involved optimizing the learning rate, batch size, weight decay, and network architecture.  Model comparison was conducted using 5-fold cross-validation and evaluation on a held-out test set.
* **Results:** The CNN significantly outperformed the FCNN, achieving a higher average accuracy (55% vs. 50%) and f1-score on the test set.  Cross-validation results confirmed the CNN's superior performance with a lower average loss (1.1941 vs. 1.2805).  Despite its increased complexity, the CNN demonstrated faster convergence during training.  Neither model exhibited significant overfitting.  See Table 1 and Table 2 in the report for detailed performance metrics.
* **Discussion:** The CNN's ability to capture spatial relationships within the Connect Four board likely contributed to its better performance.  The project demonstrates the effectiveness of convolutional architectures for tasks involving two-dimensional data representation.


## Project Assignment

The original project assignment can be found in `project_assignment.pdf`.

