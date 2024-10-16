# Autoencoder Image Compression

This project implements an **autoencoder** for image compression using the **MNIST** dataset. The autoencoder is a type of neural network that learns to encode input data into a lower-dimensional representation and then reconstructs it back to the original form. This method demonstrates the effectiveness of unsupervised learning in image compression tasks.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)

## Project Overview

The goal of this project is to develop a convolutional autoencoder that can compress images and subsequently reconstruct them while preserving the essential features. The architecture consists of two main components:

1. **Encoder:** Compresses the input image into a lower-dimensional representation.
2. **Decoder:** Reconstructs the image from the encoded representation.

## Dataset

The **MNIST** dataset is used in this project, which contains 70,000 images of handwritten digits (0-9). Each image is grayscale and has a resolution of 28x28 pixels.

- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)

## Installation

To run this project, you need to have the following libraries installed:

- TensorFlow
- NumPy
- Matplotlib

You can install the required libraries using pip:

```bash
pip install tensorflow numpy matplotlib
```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/ahmdmohamedd/autoencoder-image-compression.git
   ```

2. Navigate to the project directory:

   ```bash
   cd autoencoder-image-compression
   ```

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook autoencoder_image_compression.ipynb
   ```

4. Run the notebook cells sequentially to train the autoencoder, visualize the training process, and view the original, encoded, and reconstructed images.

## Model Architecture

The autoencoder consists of the following layers:

- **Encoder:**
  - Convolutional layers followed by max pooling layers to compress the input images.
- **Decoder:**
  - Up-sampling layers followed by convolutional layers to reconstruct the images.

## Results

After training the model, the original images, their compressed representations, and the reconstructed images are displayed for comparison. The training process can be monitored through loss metrics.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request.
