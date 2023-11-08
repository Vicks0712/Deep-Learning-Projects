# Classification of Brain Tumors with Deep Learning

## Context

In the field of medicine and medical imaging, accurate identification of brain tumors plays a critical role in the diagnosis and treatment of neurological diseases. This project focuses on the classification of brain tumor images into three main categories: glioma, meningioma and pituitary tumor, using Deep Learning techniques.

The top model, ResNet18, achieved an impressive 99% accuracy in classifying brain tumor images. This research contributes to improving accuracy and automation in brain tumor diagnosis, which could have a significant impact on medical care and patient well-being.


## Content
1. Introduction
2. Brain Tumor Dataset
3. Work environment
4. Networks and Configurations Used
5. Training Parameters
6. Loss and Precision Plots
7. Comparison between Strategies

## Brain Tumor Dataset
The data set for this project was obtained from the following source: https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset.

**However, the 'notumor' class was removed from the data set as the goal of this project is specifically to classify different types of brain tumors.**

The data set used to train and evaluate the model consists of 3,064 magnetic resonance imaging (MRI) images of brain tumors. It is divided into three classes:
* Gliomas
* Meningiomas
* Pituitary tumors.
![image](https://github.com/Vicks0712/Deep-Learning-Projects/assets/90756558/208bcc9a-b9a0-4c40-a01d-8eaf33b712c5)


## Work environment
The Weights and Biases (wandb, https://wandb.ai/site) platform was used to track the experiments in detail, including model parameters, training metrics, evaluation metrics, and visualizations. Wandb made it easy to compare multiple models and experiments in one place.

## Results
Custom models with simple architectures and pre-trained models were evaluated, such as ResNet18, MobileNet V2, AlexNet among others. Transfer learning and fine-tuning strategies were explored. The choice of optimizer and unfreezing of layers influenced the performance of the models. A summary of the results can be seen in the following table:

| Model                                          | Accuracy  |
|-----------------------------------------------|-----------|
| EfficientNet V2 S (last 5 layers unfrozen)     | 94.79%    |
| MobileNet V3 small (all layers unfrozen)      | 85.34%    |
| ResNet34 (all layers unfrozen)                | 95.44%    |
| ResNet18 (all layers unfrozen)                | 99.02%    |
| ResNet18 (3 and 4 layers unfrozen)            | 94.79%    |
| ResNet18 (last unfrozen convolutional layer)  | 96.88%    |
| ResNet18 (all weights pre-trained, no unfrozen layers) | 87.3% |
| AlexNet (all weights pre-trained, no unfrozen layers)   | 80.78%   |
| AlexNet (all layers unfrozen)                 | 96.74%    |


## Loss and Accuracy Plots of the results
Graphs are presented showing the loss and accuracy of the models throughout training. These plots provide information about the performance and stability of the models. Below you will see the development during training of the two best models obtained:

![image](https://github.com/Vicks0712/Deep-Learning-Projects/assets/90756558/f261b208-4bb6-4a02-b291-21db8a51af03)


# Usage Instructions

To utilize this code and the autoencoder model for grayscale image colorization, please follow these steps:

1. Clone this repository to your local machine.
2. Ensure that you have all the necessary dependencies installed.
3. Execute the code to either train the model or use it for image reconstruction.
4. Experiment with your own grayscale images.

# Contributions

Contributions to this project are highly encouraged and welcomed. If you wish to enhance the code, rectify errors, or introduce new features, please do not hesitate to submit a pull request.
