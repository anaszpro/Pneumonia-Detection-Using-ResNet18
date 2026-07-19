## Pneumonia-Detection-Using-ResNet18
This project utilizes a pre-trained ResNet-18 model for pneumonia detection from chest X-ray images. It classifies images into Normal or Pneumonia using transfer learning, with a curated dataset divided into training and validation sets. The model is fine-tuned, robust, and evaluated for accuracy, precision, recall, and F1-score.

##Pneumonia Detection using ResNet-18
This project demonstrates a deep learning-based approach to detecting pneumonia from chest X-ray images using a pre-trained ResNet-18 model. The model has been fine-tuned for binary classification (Normal vs. Pneumonia) using a curated dataset of X-ray images. This project highlights the power of transfer learning to address real-world medical challenges and offers an end-to-end pipeline for training, evaluation, and inference.

##Features
#1. Data Preparation
Dataset: The dataset is organized into training (new_train) and validation (new_val) subsets.
Preprocessing:
Data augmentation techniques such as random resizing, cropping, and horizontal flipping for robustness.
Normalization using ImageNet's standard mean and standard deviation.
#2. Model Architecture
Base Model: ResNet-18, pre-trained on the ImageNet dataset.
Fine-Tuning:
The final fully connected layer is replaced to accommodate binary classification.
Earlier layers are frozen to retain learned features while minimizing computational cost.
#3. Training
Loss Function: CrossEntropyLoss is used to compute classification error.
Optimizer: Adam optimizer with a custom learning rate and weight decay.
Metrics: Accuracy, precision, recall, and F1-score are tracked for both training and validation sets.
#4. Evaluation
Classification performance is evaluated using a detailed report on the validation set.
Metrics like accuracy and loss are computed for each epoch.
#5. Inference
The trained model can predict outcomes for unseen chest X-ray images.
Outputs include the predicted class (Normal/Pneumonia) with the input image visualized alongside its label.
#6. Deployment
The model and pipeline are designed to run efficiently in Google Colab with GPU acceleration.
Integration with Google Drive ensures seamless dataset and model checkpoint management.
##Technical Stack
P#rogramming Language: Python
#Libraries: PyTorch, torchvision, sklearn, PIL, NumPy, Matplotlib
#Tools: Google Colab, Google Drive
#Hardware: Supports GPU acceleration via CUDA
##Getting Started
Clone the repository.
Upload your dataset and modify paths as needed.
Train the model using the provided training loop.
Evaluate and test the model on unseen data.
##Project Goals
Develop an accurate and efficient pneumonia detection model.
Leverage transfer learning to reduce training time and enhance performance.
Provide a comprehensive framework for real-world medical image classification tasks.
