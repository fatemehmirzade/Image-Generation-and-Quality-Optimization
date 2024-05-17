# Diffusion-model
The provided code establishes and trains a diffusion model utilizing the CIFAR-10 dataset, focusing on generating high-quality images. The following is a structured and academic overview of the process:

Utility Functions: Several utility functions are defined, including those for converting images to tensors, reversing the conversion, and reshaping tensors for feature mapping.

Training Parameters and Device Configuration: Training parameters such as the number of steps, batch size, learning rate, and device (GPU or CPU) are configured.

Data Loaders: Data loaders for the CIFAR-10 dataset are established to streamline the training and testing processes.

Diffusion Functions: Functions are defined to model the diffusion process by introducing noise to images at various steps.

Image Visualization: The code periodically saves and visualizes images at different stages of the diffusion process to monitor progress.

U-Net Model Definition: A U-Net model, specialized for image generation, is defined. This neural network architecture is pivotal for the task.

Training Loop: The U-Net model is trained using the specified parameters. The training loop includes tracking the loss and saving the best-performing model based on validation metrics.

Image Generation: Post-training, the model generates images from random noise inputs. These generated images are saved for further evaluation.

FID Score Calculation: The Fréchet Inception Distance (FID) score is computed to assess the quality of the generated images in comparison to real CIFAR-10 images.

In summary, the code systematically sets up the environment, trains a diffusion model on CIFAR-10 data, generates new images, and evaluates their quality through quantitative metrics. This structured approach ensures a comprehensive workflow from data preparation to model evaluation.

The result:  ![image](https://github.com/fmirzadeh99/Diffusion-model/assets/169579231/bc95ff0b-7d48-465f-bca6-a7f73d222e65)
