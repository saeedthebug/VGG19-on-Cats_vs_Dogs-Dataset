# Cat vs Dog Image Classifier using VGG19 Model

This project was assigned to me by the Government Innovation Lab (GIL) Quetta, Pakistan. The task was to take any dataset from Kaggle and train a VGG19 or Inception model. I decided to use the Cats vs Dogs dataset (http://www.kaggle.com/c/dogs-vs-cats/data) from Kaggle.

## Data Preprocessing

After reading all the related work, I noticed that the highest accuracy achieved on this dataset was 97% with the complete dataset. To challenge myself, I decided to use less than 10% of the data and then split it into three parts. I used 2000 images for training, 1000 for validation, and 1000 for testing from the original 25,000 image dataset.
Model Training

After preprocessing the dataset and using data augmentation techniques, I trained the VGG19 model. I achieved a training accuracy of 96%, validation accuracy of 95%, and testing accuracy of 95%.

## Model Evaluation

After training and evaluating the model, I saved it as "vgg19.model" and in HDF5 format as "my_model.h5".

## Deployment

In the "deploy_raspberrypi" directory, there is a Python file named "vgg19_raspberryPi.py". To run this program on a Raspberry Pi, you need to do two things:

    Install any operating system on your SSD card and insert it into the Raspberry Pi.

    Install the following dependencies:
        OpenCV (cv2)
        TensorFlow
        NumPy
        Keras (will be inside TensorFlow by default)

