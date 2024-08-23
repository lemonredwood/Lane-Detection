Precision Lane Detection with SegNet: Multi-Scale Features and Attention
Overview

This repository contains the code and resources for the project "Precision Lane Detection with SegNet: Multi-Scale Features and Attention." The project aims to develop a highly accurate and computationally efficient lane detection model tailored for autonomous vehicles by leveraging custom modifications of the U-Net and SegNet architectures.
Objective

The primary objective is to create a novel architecture that balances precision and real-time performance, specifically addressing the challenges posed by varying lighting conditions, diverse road surfaces, and limited labeled data. Accurate lane detection is a critical component for safe and reliable navigation in autonomous vehicles.
Key Features

    Custom Modifications: Incorporates spatial and channel attention mechanisms to enhance the focus on lane regions.
    Multi-Scale Feature Extraction: Utilizes pyramid pooling and atrous convolution to capture context at various scales.
    Loss Functions: Employs boundary-aware, dice, and focal loss functions for accurate lane edge detection and handling class imbalance.
    Extreme Condition Handling: Expands the training dataset to improve performance in extreme weather and lighting conditions.

Proposed Architecture

The project builds upon the SegNet architecture, a deep learning model designed for semantic segmentation tasks. It features an encoder-decoder structure optimized for retaining spatial information and reducing computational overhead.

    Encoder: Captures and compresses feature maps through convolutional and max-pooling layers, storing max-pooling indices for accurate upsampling.
    Decoder: Uses stored max-pooling indices to upsample the feature maps, ensuring accurate localization of features in the segmented output.
    Pixel-wise Classification: The final layer generates segmented output through pixel-wise classification.
