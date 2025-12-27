# Image Preprocessing Pipeline for AI
# 1- Dataset Selection:
This project uses the CIFAR-10, a publicly available dataset containing 60,000 color images across 10 classes.
Two images were selected from the dataset:
Image 1: Airplane
Image 2: Automobile

# Image Properties:
Size: 32 × 32 pixels
Channels: 3 (RGB)
Pixel Value Range: [0, 255]
The dataset is loaded programmatically using PyTorch’s torchvision library; no manual image upload is required.

# 2- Preprocessing Pipeline
The following preprocessing steps were applied to both images:
Resize – Images resized to 64 × 64 to standardize input size
Grayscale Conversion – Reduced color channels to simplify features
Rotation – Applied random rotation to simulate orientation variance
Horizontal Flip – Introduced data augmentation
Normalization – Scaled pixel values to the range [-1, 1] for AI models
Bonus: Custom Sharpening Filter – Enhanced edges using a kernel-based filter

# 3- Analysis of Each Step:
For every preprocessing step:
The transformation was applied to both images
Outputs were visualized side-by-side

Image shape and pixel value range were printed

Normalization and sharpening were retained for model input, while de-normalization was used only for visualization to ensure clarity.
