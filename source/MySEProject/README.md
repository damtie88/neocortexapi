# Multi-Sequence Learning with Language Semantic

## Overview

This project demonstrates the implementation of Multi-Sequence Learning, specifically focusing on sequences of language semantics. The goal is to train a model to learn sequences from a given text file and predict subsequent elements in the sequence. The model is based on the NeoCortexApi and includes both Spatial Pooling (SP) and Temporal Memory (TM) components.

## Files

- **Program.cs**: Contains the main entry point and experiment setup. It initiates the learning process and demonstrates how to use the implemented methods.
- **MultisequenceLearning.cs**: Implements the core Multi-Sequence Learning experiment. It includes the training of the Spatial Pooler (SP) and Temporal Memory (TM) and provides methods for running the experiment with different sequences.

## How to Run

1. Open the project in a C# development environment, ensuring you have the necessary dependencies installed.

2. Run the `Main` method in `Program.cs` to start the experiment.

## Experiment Details

### Learning from Text Sequences

1. **Sequence Representation**: The sequences are represented as arrays of ASCII codes of characters in the provided text. Control characters such as `\r`, `\n`, `\t` are removed.

2. **Training and Testing Data**: The learning sequences are read from a file, and the data is split into two groups: 90% for training and 10% for testing.

3. **Training the Model**: The model is trained using the training data. The learning process involves both SP and TM components.

4. **Evaluation**: The accuracy of the model is evaluated using binary cross-entropy, comparing expected bits in the Spatial Distributed Representation (SDR) with predicted probabilities.

### Prediction and Text Completion

1. **Predictive Capability**: After training, the model can predict the next element in a sequence. The prediction accuracy is assessed using the testing data.

2. **Text Completion**: Users can enter a text, and the model will generate the continuation of the text based on its learned patterns.

3. **Variety in Predictions**: The model supports generating different sequences, providing diverse predictions beyond the character with the maximal probability.

## Results and Output

- The experiment output includes information on the learning process, cycle details, matches, and prediction accuracy.

- The README provides an overview of the project, details on running the experiment, and insights into the implemented features.

## Dependencies

- This project relies on the NeoCortexApi library for implementing the Spatial Pooler (SP) and Temporal Memory (TM) components.




