# Glaucoma Progression Predicition

This project investigates whether a single retinal nerve fiber layer thickness (RNFLT) map can be used to predict future glaucoma progression using deep learning.

# Goal

Predict whether an eye will show future glaucomatous progression based on a baseline RNFLT map.

# Methods

Input: Single-channel RNFLT map (225×225)
Task: Binary classification (Progression vs No progression)

# Models tested:

VGG16-BN

EfficientNet-B0

Both customized for single-channel OCT input.

# Training setup:

Loss: BCEWithLogitsLoss (+ class-imbalance weighting)

Optimizer: AdamW

LR: 5e-5

Batch size: 32
