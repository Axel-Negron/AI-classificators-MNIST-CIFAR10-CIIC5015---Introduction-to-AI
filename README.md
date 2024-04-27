**Project Title:** MNIST and CIFAR10 Classifiers with PyTorch

**Overview**

This project explores the development of image classification models using the PyTorch framework. It contains implementations for several convolutional neural network (CNN) architectures designed to classify images from the MNIST (handwritten digits) and CIFAR10 (common objects) datasets.

**Key Features**

* **Diverse Models:** The repository includes these models:
    * **MNIST:**
        * Simple CNN with convolutional layers
        * CNN with multiple convolutional blocks
        * CNN with Batch Normalization and Max Pooling    
    * **CIFAR10:**
        * Baseline CNN with convolutional layers
        * CNN with deeper architecture and convolutional blocks
        * A more advanced CNN (Bonus CIFAR10 model) incorporating smaller kernels, increased channels, and Batch Normalization.

* **Data Loading:** Custom functions (`get_MNIST_data`, `get_CIFAR10_data`) handle dataset downloading, preprocessing, and the creation of data loaders.

* **Training and Testing:** The code provides functionality for training models, saving trained weights, and evaluating their performance on test datasets.

* **Time Profiling:** The code includes basic time profiling to measure the training time of each model. You can find the training times listed in the `time_log.txt` file. 

**Code Structure**

The code is organized into cells (indicated by `%%`) for flexibility using jupyter notebook. Here's a breakdown:

1. **Imports:** Import necessary PyTorch modules and set up constants.
2. **Data:**  Functions for loading and preparing MNIST and CIFAR10 datasets.
3. **Models:**  Implementation of the various CNN architectures.
4. **Functions:**  Helper functions for model loading and the core training/testing loop.
5. **Main Execution:**
    * Models are retrieved (or created if not already trained).
    * Untrained models undergo training.
    * All models are tested.
    * Training times are logged into  `time_log.txt`.

**How to Run**

1. **Prerequisites:**
    * Python 3.x
    * PyTorch (refer to the official PyTorch website for installation: https://pytorch.org/)
    * torchvision

2. **Clone:** Clone this repository.

3. **Execute:** Run the code cells in order. You may run it in a Jupyter Notebook environment or execute it as a Python script.

**Results**

Training and testing results are printed to the console. Evaluation metrics (loss and accuracy) for each model are displayed. Additionally, a `time_log.txt` file is generated containing the training times for each model.

**Contributions**

Contributions are welcome! Feel free to open issues, submit pull requests, or suggest new model implementations. 
