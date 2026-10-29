
# Underwater Image Detection Using Machine Learning

## Project Overview
This project uses deep learning to classify underwater images into two
categories: Fish and No fish.

It uses transfer learning with MobileNetV2, a convolutional neural
network pretrained on ImageNet.

## Objectives
- Classify underwater images as Fish or No fish.
- Apply transfer learning to image classification.
- Evaluate the model using accuracy, precision, recall, and F1-score.
- Test predictions on new images.

## Technologies Used
- Python
- TensorFlow and Keras
- MobileNetV2
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Model Workflow
1. Collect and label underwater images.
2. Resize images to 224 x 224 pixels.
3. Normalize pixel values.
4. Split data into training and validation sets.
5. Train a classification head using MobileNetV2 features.
6. Evaluate the model.
7. Predict the class of a new image.

## Dataset
The initial experiment uses 200 images:
- 100 Fish images
- 100 No fish images

The data is split into 160 training images and 40 validation images.

## Preliminary Results
- Validation accuracy: 97.5%
- Validation images: 40
- Correct predictions: 39 out of 40

These are preliminary results from a small validation set. More images
and testing on an independent dataset are needed to assess generalization.

## Model
The trained model is saved as:
`models/underwater_classifier.keras`

## How to Run
1. Open `Underwater_Image_Detection.ipynb` in Google Colab.
2. Run the notebook cells in order.
3. Train or load the model.
4. Upload an underwater image to test a prediction.

## Project Structure
underwater-image-detection/
- Underwater_Image_Detection.ipynb
- README.md
- models/
- results/
  - training_history.png

## Future Improvements
- Increase the size and diversity of the dataset.
- Evaluate on a separate test set.
- Add data augmentation.
- Test performance on different underwater environments.
- Consider multi-class classification for more marine species.

## Disclaimer
This is an educational machine learning project. Predictions may be
incorrect, especially on images that differ from the training data.
