# Brain Tumor Detection via CNN

This repository contains a Deep Learning project for automated brain tumor detection using MRI scans. The model leverages a Convolutional Neural Network (CNN) to achieve high-accuracy binary classification.

## Dataset
The dataset comprises 253 Brain MRI images:
- **Tumorous:** 155 images
- **Non-tumorous:** 98 images

## Model Architecture
The CNN is built using the Keras Sequential API and includes:
- **Convolutional Layers (Conv2D):** For spatial feature extraction.
- **Batch Normalization:** To improve training speed and stability.
- **Pooling (MaxPooling2D):** For spatial variance and dimensionality reduction.
- **Regularization (Dropout):** To mitigate overfitting during training.
- **Output Layer:** A Dense layer with Sigmoid activation for binary classification.

##  Key Features
- **Visual EDA:** Includes plotting of MRI samples for both classes.
- **Evaluation:** Features a confusion matrix and detailed classification reports (Precision, Recall, F1-score).
- **Interactive Prediction:** An integrated tool to upload local MRI images and receive instant predictions with confidence scores.
- **Colab Optimized:** Pre-configured for Google Colab environments using GPU acceleration.

## Model Architecture
<img width="1000" height="535" alt="image" src="https://github.com/user-attachments/assets/55267361-c44b-4e60-a69e-f8a06d2ff2ec" />

## Requirements & Tech Stack
- **Languages:** Python
- **Frameworks:** TensorFlow, Keras
- **Libraries:** NumPy, Pandas, OpenCV (`cv2`), Matplotlib, Seaborn, Scikit-learn, PIL

## Setup and Requirements
The following libraries are required:
- `tensorflow`
- `keras`
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `opencv-python`
- `scikit-learn`

## How to Use
1. Open the brain_tumor.ipynb uploaded in the current repositary
2. Run the library import and setup cells.
3. Upload your dataset (expected as `BTC.zip`) when prompted.
4. Execute the training cells to build the model.
5. Use the "Interactive Prediction" cell to test the model with your own MRI images.
6. The zip file and the ipynb file is provided in the project folder

## Future Advancements
- **Transfer Learning:** Integrating pre-trained models like ResNet50 or VGG16 for performance benchmarking.
- **Dataset Augmentation:** Implementing advanced augmentation techniques to improve model generalization.
- **Explainable AI (XAI):** Adding Grad-CAM visualizations to highlight the specific tumorous regions identified by the model.
- **Grad-CAM Integration:** Implementing Gradient-weighted Class Activation Mapping to show heatmaps of exactly where the model "sees" the tumor

## License
This project is provided under the **Apache License 2.0**. .
