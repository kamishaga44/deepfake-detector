# Deepfake Detection Web Service

A web application for detecting AI-generated and manipulated images using deep learning.

## Overview

This project was developed as a diploma project to explore how deep learning can support digital security by distinguishing real images from AI-generated or manipulated images.

The application provides a web interface where users can upload an image for analysis.

## Models

The project uses two image classification models:

- **DeepfakeCNNv3** — a custom convolutional neural network.
- **EfficientNet-B0** — a model based on a pretrained architecture.

The trained model weights (`.pth` files) are not included in this public repository.

## Technologies

- Python
- Flask
- PyTorch
- Torchvision
- Pillow
- HTML and CSS

## Features

- Image upload and validation
- Image classification using two models
- Prediction result and confidence score
- Separate interfaces for the two models
- Information pages about the application

## Local Setup

1. Clone this repository.
2. Create and activate a Python virtual environment.
3. Install the required dependencies.
4. Place the trained model files in the project root directory:
   - `deepfake_model_v3.pth`
   - `deepfake_efficientnet.pth`
5. Run the application:

```bash
python app.py
```

The trained model files are private and must be obtained separately. Prediction endpoints will not work until the corresponding model weights are available.

## Disclaimer

This project is intended for educational and research purposes. Predictions should not be treated as definitive proof that an image is real or AI-generated.