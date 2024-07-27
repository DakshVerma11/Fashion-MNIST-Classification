# Fashion MNIST Classification

This repository contains a neural network model built using TensorFlow for image classification on the Fashion MNIST dataset.

## Project Overview

The objective of this project is to classify images of fashion items into one of ten categories. The model is trained on the Fashion MNIST dataset, which consists of 70,000 grayscale images of fashion products, with each image being 28x28 pixels. 


## Dataset

The dataset used is [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) provided by Zalando. It includes the following categories:
![image](https://github.com/user-attachments/assets/2d34a1ab-9d1b-463d-af3f-313e10021cb6)


| Label | Class       |
|-------|-------------|
| 0     | T-shirt/top |
| 1     | Trouser     |
| 2     | Pullover    |
| 3     | Dress       |
| 4     | Coat        |
| 5     | Sandal      |
| 6     | Shirt       |
| 7     | Sneaker     |
| 8     | Bag         |
| 9     | Ankle boot  |


## Model Architecture

The model is a neural network with the following layers:

1. **Flatten Layer**: Converts the 28x28 pixel images into a 1D array.
2. **Dense Layer 1**: 1024 neurons, ReLU activation.
3. **Dense Layer 2**: 256 neurons, ReLU activation.
4. **Dense Layer 3**: 64 neurons, ReLU activation.
5. **Output Layer**: 10 neurons, softmax activation for classification.

## Training

The model is trained for 50 epochs using the Adam optimizer and Sparse Categorical Crossentropy loss function.

## Installation

To run the code, you need to install the required libraries:

```bash
pip install tensorflow tensorflow_datasets
```

## Usage

To train the model, execute the following steps:

1. Load the Fashion MNIST dataset.
2. Normalize the images.
3. Define and compile the model.
4. Train the model on the training dataset.

## Results

The model achieves high accuracy on the test dataset, demonstrating its effectiveness in classifying fashion items. The model achieved an accuracy of 89.84% on the test dataset.

![image](https://github.com/user-attachments/assets/906fc73c-1581-4346-a9f6-cb9b6892a620)


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [TensorFlow](https://www.tensorflow.org/)
- [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) by Zalando
