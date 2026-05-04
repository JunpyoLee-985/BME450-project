# Title

Deep Learning-Based Detection of Mitral Regurgitation from Echocardiography Images

## Team members

Junpyo Lee (JunpyoLee-985)

## Project description

# Title

Deep Learning-Based Detection of Cardiomegaly from Chest X-ray Images

## Team members

Junpyo Lee (JunpyoLee-985)

## Project description

This project aims to train a deep learning model to detect cardiomegaly from chest X-ray images. Cardiomegaly is a condition in which the heart appears enlarged on chest radiographs. The task is formulated as a binary image classification problem with two classes: normal and cardiomegaly.

The original project idea was to detect Mitral Regurgitation (MR) from echocardiography images. However, this topic was changed because it was difficult to find an easily accessible, pre-labeled MR image dataset suitable for a simple image classification project. MR diagnosis often depends on echocardiography videos, color Doppler information, and clinical interpretation, which made the dataset preparation more complex. Cardiomegaly was chosen instead because it can be studied using single chest X-ray images, and a labeled Kaggle dataset was available for binary classification.

The dataset was downloaded from Kaggle and organized into PyTorch ImageFolder format. The original labels used true/false folders, where false was treated as normal and true was treated as cardiomegaly. To keep the dataset balanced, 1,500 images were used from each class. The final dataset contained 2,100 training images, 450 validation images, and 450 test images.

A simple convolutional neural network (CNN) was trained using PyTorch. The model used three convolutional layers followed by fully connected layers. The images were resized to 128 × 128 pixels, and the model was trained using CrossEntropyLoss and the Adam optimizer.

The results include training loss, validation loss, validation accuracy, final test accuracy, and example prediction images. After 15 epochs, the final test accuracy was 70.00%. This project is intended as an educational proof-of-concept model, not as a clinical diagnostic system.

Large raw image datasets and model weight files are not included in this repository due to file-size restrictions.
