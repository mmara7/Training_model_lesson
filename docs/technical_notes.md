# Technical Notes

## CNN Basics
- **Conv2D:** detects local patterns in images
- **MaxPooling2D:** reduces spatial dimensions
- **Flatten:** converts 2D feature maps to 1D vector
- **Dense:** fully connected layer, computes class scores
- **Softmax:** converts outputs to probabilities

## Preprocessing
- Resize images to a fixed size (e.g., 32x32)
- Normalize pixel values to [0,1]
- One-hot encode labels for classification
