# Tumor-Detection-in-MRI-Images-using-CNN
This repository contains a Convolutional Neural Network (CNN) model implemented in TensorFlow, which can be used for detecting tumors in MRI images. The model has been trained using a dataset of 4370 MRI images (2475 with tumors and 1895 without tumors) that can be accessed via the following Google Drive link: https://drive.google.com/drive/folders/1Y2X452rGgjiGwb7uTn9M4xelANWqFp4J

### Requirements
The model has been developed using Python 3.8 and TensorFlow 2.5.0. To run the Jupyter Notebook file, you will need to install the following packages:

- TensorFlow 2.5.0
- NumPy
- Matplotlib

### Usage
To use the model, please follow these steps:

1. Download the dataset from the Google Drive link provided above and extract it to a folder called data in the root directory of the project.
2. Open the Jupyter Notebook cnn.ipynb using Jupyter Notebook or a similar environment.
3. Run the cells in the notebook in sequential order to train the model, evaluate its performance, and generate predictions for new MRI images.

### Model Architecture
The CNN model used for tumor detection in MRI images consists of several convolutional, pooling, and fully connected layers. The architecture of the model is as follows:

- Input layer (with the shape of each MRI image as the input shape)
- rescaling layer
- Convolutional layer (16 filters with a kernel size of 3x3 and ReLU activation)
- Max pooling layer (with a pool size of 2x2)
- Convolutional layer (32 filters with a kernel size of 3x3 and ReLU activation)
- Max pooling layer (with a pool size of 2x2)
- Convolutional layer (64 filters with a kernel size of 3x3 and ReLU activation)
- Max pooling layer (with a pool size of 2x2)
- Dropout layer (with a rate of 0.)
- Flatten layer
- Fully connected layer (128 units with sigmoid activation)
- Output layer (with 1 unit and sigmoid activation)
- Results

The trained model achieved an accuracy of approximately 98% on the test set, indicating that it is capable of accurately detecting tumors in MRI images.

### Credits
This project was developed by Ilyas KHIAT as part of his TIPE module to enter French Grande École (higher education institution) located in Bordeaux. If you use this code or dataset, please consider citing this repository.

### License
This project is licensed under the MIT License - see the LICENSE file for details.
