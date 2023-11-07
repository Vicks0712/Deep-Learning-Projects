# Image Scaling Autoencoder

An autoencoder is a type of neural network used to learn a compact representation of a dataset, such as images. In the case of using an autoencoder to upscale an image, a specific autoencoder architecture known as an **image scaling autoencoder** can be employed.

## Advantages
- Allows the generation of higher-resolution images from lower-resolution ones without the need for pixel interpolation techniques, enhancing the quality of the final image.
- Using an autoencoder to learn a compact image representation can yield higher-quality results compared to other image upscaling methods.

## Libraries Used

Below are some of the most important libraries used in this project:

- PyTorch: An open-source deep learning library that simplifies the creation and training of neural networks.
- torchvision: A PyTorch extension providing datasets and pre-trained models for computer vision tasks.
- NumPy: A library for mathematical and numerical operations in Python.
- Matplotlib: A library for creating data visualizations and graphs.
- scikit-learn: A library that provides tools for machine learning and data mining.

Make sure to have these libraries installed in your development environment before running the code.

## DataLoader
We have utilized the MNIST dataset for training and validating these models. To load the data, we used PyTorch DataLoader. Here is an example of how to load the training data:

```
transform = transforms.ToTensor()
mnist_data = datasets.MNIST(root='./data', train=True, download=True, transform=transform)
data_loader = torch.utils.data.DataLoader(dataset=mnist_data, batch_size=64, shuffle=True)
```

## Model
We have implemented an autoencoder model: one for upscaling from 7x7 to 28x28. Here is a brief definition of it:

#### Autoencoder_7 (7x7 to 28x28)
This autoencoder consists of two main parts: the encoder and the decoder. The encoder takes the input image of size 7x7 and reduces it to a compact representation, while the decoder takes this compact representation and reconstructs the image to the original size of 28x28.

## Training
You can train the model using your data or the MNIST dataset. Adjust the number of epochs and other hyperparameters as needed for your project. Here is an example of how to train the model:

## Results
Below are two theoretical images illustrating the expected results of each of the two autoencoder models:

![image](https://github.com/Vicks0712/Deep-Learning-Projects/assets/90756558/cbce072c-0de7-4812-a0f3-f366030c722a)

**Note:** These images depict theoretical results. Actual results may vary based on the dataset and specific use case. Ensure that you evaluate the model's performance with real data and document the actual results obtained in this section.

## Usage Instructions

To use this code and the autoencoder model for grayscale image colorization, please follow these steps:

1. Clone this repository to your local machine.
2. Ensure that you have all the necessary dependencies installed.
3. Execute the code to either train the model or use it for image resolution enhancement.
4. Experiment with your own images.

## Contributions
If you wish to contribute to this project, we encourage your involvement. You can contribute in the following ways:

- Reporting issues or bugs.
- Proposing improvements or new features.
- Submitting pull requests to fix issues or implement new features.
