# Animal Species Recognition Project

## Overview

This project utilizes a pre-trained deep learning model (ResNet50) to predict the species of an animal from an image. The model is based on the ResNet50 architecture and is trained on the ImageNet dataset, enabling it to recognize a wide variety of objects, including animals. The project leverages TensorFlow and Keras to perform image classification tasks.

## Requirements

To run this project, you need the following Python libraries installed:

- `tensorflow`
- `numpy`
- `Pillow` (for image processing)

You can install the required libraries using the following command:

```bash
pip install tensorflow numpy Pillow
```

### Project Structure
Animal-Species-Recognition/</br>
│</br>
├── images/                    # Directory to store test images</br>
│   └── test_image.jpg         # Example image file for prediction (replace with your own image)</br>
│</br>
├── main.py         # Python script to predict animal species from an image</br>


### Usage

Ensure that the required libraries are installed.</br>
Place the image you want to classify in the images/ directory.</br>
In the predict_species.py script, set the img_path variable to the path of your image (e.g., 'images/test_image.jpg').</br>
Run the script using Python:</br>
```bash
python predict_species.py
```
The script will output the top 3 predicted labels for the image along with their corresponding confidence scores.


## Code Explanation
### Model Loading:

The pre-trained ResNet50 model is loaded with ImageNet weights. ResNet50 is a deep convolutional neural network known for its high accuracy in image classification tasks.</br>

### Image Preprocessing:

The image is resized to 224x224 pixels, the required input size for ResNet50.</br>
The image is then converted into a format suitable for the model by using preprocess_input.</br>

### Prediction:

The model predicts the species by classifying the input image.</br>
The top 3 predictions are decoded and printed with their associated confidence scores.</br>

### Example Output: 

```
Prediction 1: Labrador_retriever (0.64)
Prediction 2: bloodhound (0.10)
Prediction 3: English_foxhound (0.08)
```
