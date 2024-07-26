# Diffusion-model

## Introduction
This project sets up and trains a diffusion model on the CIFAR-10 dataset with a focus on high-quality image generation. Structurization of this project workflow can be done in three different components: data preparation, model training itself, and result evaluation.

![image](https://github.com/user-attachments/assets/39e24388-ef59-4597-a5cd-14b301c06093)
|:-:|
|Overview of Diffusion Models

## Data Preparation
Utility Functions
Several utility functions are defined for data handling and transformation:
Converting images to tensors and vice versa.
This is tensor reshaping for feature mapping purposes.
Data Loaders
It establishes data loaders for the CIFAR-10 dataset to enable smooth training and testing by efficiently handing over data in batches.

## Hyperparameters and Training
Parameters of Training and Configuration of Devices
Key training parameters are configured, including:
Number of steps
Batch size
Learning Rate
Device Selection (GPU or CPU)
Diffusion Functions
These functions are designed for the process of diffusion by adding noise to the images at different steps during this process. This step is an essential part of training a diffusion model.

![image](https://github.com/user-attachments/assets/470a4c48-5c0d-45f6-8b7b-a79fcac0eb77)
|:-:|
|Adding Noise

## U-Net Model Definition
A class, image generation, specialized with a U-Net model has been defined. This neural network architecture is paramount in the generation of high-quality images.

![image](https://github.com/user-attachments/assets/f557aead-9eea-49c9-80ee-685bd9e4bd50)
|:-:|
|Unet diagram

## Training Loop
The U-Net model will now be trained for the specified parameters. During training:
The losses are accounted for to keep track of the progress. It saves the best model based on validation metrics.

![image](https://github.com/user-attachments/assets/c184e9fa-6109-4fcd-b9b2-1ae34a3f7674)
|:-:|
|Training Loss Curve

## Image Visualization
The code periodically saves and visualizes images during training at different stages of this diffusion process to monitor progress and check the quality of images.

## Evaluation Metrics and Results Image Generation
It will generate images after training, based on random noise as an input. All the generated images will be saved for further evaluation. Quality Assessment It runs the Fréchet Inception Distance score, which evaluates the quality of generated images compared to real CIFAR-10. The FID score quantifies how similar generated images are to their original dataset. Conclusion It sets up the environment, trains a diffusion model on CIFAR-10 to generate new images, and finally evaluates their quality. It means such a well-structured workflow from data preparation to model evaluation shall not miss a single step, focusing only on high-quality image generation.



