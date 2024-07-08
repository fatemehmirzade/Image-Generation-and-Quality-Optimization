# Diffusion-model
The provided code sets up a diffusion model on CIFAR-10 data and trains it, where image quality is the most important consideration. The well-structured and academic overview of what this code does shall be provided below: Utility Functions: A few utility functions have been defined, such as those for converting images into tensors, reverting that conversion back to images, and reshaping tensors for purposes connected with feature mapping. Training Parameters and Device Configuration: Training parameters such as the number of steps, batch size, learning rate, and device (GPU or CPU) are configured.

Data Loaders: Data loaders for the CIFAR-10 dataset are established to streamline the training and testing processes.
Diffusion Functions: Functions are defined to model the diffusion process by introducing noise to images at various steps.

Image Visualization: The code periodically saves and visualizes images at different stages of the diffusion process to monitor progress.
U-Net Model Definition: A U-Net model, specialized for image generation, is defined. This neural network architecture is pivotal for the task.
Train the U-Net model with the given parameters. In this section of the training loop: track the losses and save the best model as per validation metrics.
Image Generation: This is a model under which images are generated against random noise inputs after training. The generated images are saved for further evaluation.

It calculates the FID score, which is a measure of the quality of generated images, compared to real CIFAR-10 images. Precisely, this code programmatically configures the environment, trains a diffusion model in CIFAR-10 data, generates new images, and measures their qualitative values. On top of that, such a well-structured way to ensure a comprehensive workflow from data preparation to model evaluation is followed.

The result:  ![image](https://github.com/fmirzadeh99/Diffusion-model/assets/169579231/bc95ff0b-7d48-465f-bca6-a7f73d222e65)
