# Extracting Supernova Signals

## Overview
This project focuses on extracting supernova signals from noisy data using a combination of data processing, machine learning, and signal processing techniques. The primary goal is to develop a neural network model that can identify and isolate supernova signals within a dataset that includes various forms of noise.

## Key Technologies and Libraries

### Data Processing and Visualization
- **Pandas**: Used for data manipulation and analysis, including reading, filtering, and visualizing the dataset.
- **Matplotlib**: Utilized for plotting the data to visualize and analyze the signals effectively.

### Noise Generation
- **Bilby**: A Bayesian inference library for gravitational-wave astronomy, used to generate noise from the LIGO-Hanford (H1) interferometer data.
- **Numpy**: Employed for numerical operations, including the generation of white noise and color noise to simulate real-world noisy environments.

### Machine Learning
- **PyTorch**: A deep learning framework used to build and train neural network models. It provides the tools necessary for creating an autoencoder to extract features from the signal data.
- **Autoencoder Model**: A neural network model designed for dimensionality reduction and feature extraction. The autoencoder helps in identifying patterns within the noisy data that correspond to supernova signals.

### Data Loading
- **PyTorch DataLoader**: Facilitates efficient data handling by batching the data for training, validation, and testing the neural network model.

### Signal Processing
The project involves advanced signal processing techniques to analyze and process the signal data. This includes noise filtering, transformation, and feature extraction to isolate the supernova signals.

## Project Workflow
1. **Data Loading**: Load the dataset and perform initial preprocessing steps such as filtering out flat signals and visualizing the data.
2. **Noise Generation**: Generate realistic noise using Bilby and Numpy to simulate the environment in which supernova signals are detected.
3. **Model Building**: Construct an autoencoder neural network using PyTorch. The model is designed to learn and extract meaningful features from the noisy signal data.
4. **Data Batching**: Utilize PyTorch's DataLoader to batch the data for efficient training, validation, and testing.
5. **Training and Evaluation**: Train the autoencoder model on the noisy dataset and evaluate its performance in isolating and identifying supernova signals.

## Requirements
- Python 3.x
- Pandas
- Matplotlib
- Bilby
- Numpy
- PyTorch

## Conclusion
This project demonstrates the application of machine learning and signal processing techniques to extract supernova signals from noisy data. By leveraging advanced tools and libraries, the project aims to contribute to the field of gravitational-wave astronomy and enhance our ability to detect and analyze cosmic events.
