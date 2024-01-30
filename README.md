Fetal Head Segmentation Using U-Net - Project Readme
Overview
This project involves the implementation of a U-Net architecture for fetal head segmentation in ultrasound images, using PyTorch. The project showcases the application of deep learning in medical image analysis, particularly in segmenting fetal heads from ultrasound images.

Key Features
Technology Stack: Utilizes libraries like NumPy, PyTorch, OpenCV, PIL, Pandas, and OS.
Architecture: The U-Net model comprises 23 convolutional layers, tailored for detailed image segmentation.
Image Resolution: Processes images of size 572x572 pixels.
High Accuracy: Achieves a Dice score of 95.6% on the test set and a pixel-to-pixel accuracy of 97.4%.
Hardware Used: Training and inference performed on an RTX 3080 Ti GPU.
Data Augmentation: Includes random rotations, horizontal flips, and vertical flips to enhance model robustness.
Dataset Size:
Training: 799 images
Validation: 200 images
Testing: 335 images
Binary Segmentation: Predicts binary masks for segmenting the fetal head.
Loss Plotting: Visualizes training and validation loss over epochs.
Early Stopping: Implements early stopping with checkpoints for saving the best model weights.
Learning Parameters
Learning Rate: 0.01
Batch Size: 2
Implementation Details
U-Net Model: The U-Net model is designed specifically for medical image segmentation. The architecture includes a downsampling path to capture image context and an upsampling path for precise localization.
Loss Function: A combination of Binary Cross Entropy and Dice Loss is used to compute the loss, optimizing both pixel accuracy and overlap.
Performance Metrics: Dice score and pixel-to-pixel accuracy are the primary metrics for evaluating model performance.
Usage
Setup: Install required Python libraries (NumPy, PyTorch, OpenCV, PIL, Pandas, OS).
Data Preparation: Collect and preprocess ultrasound images of fetal heads along with their corresponding segmentation masks.
Training: Train the U-Net model on the prepared dataset. Monitor training and validation loss.
Evaluation: Evaluate the model on the test set using metrics like Dice score and pixel-to-pixel accuracy.
Inference: Use the trained model for segmenting fetal heads in new ultrasound images.
Additional Information
Data Augmentation: To ensure the model generalizes well, data augmentation techniques like random rotations and flips are utilized.
Early Stopping and Checkpoints: Early stopping prevents overfitting, and checkpoints save the model with the best validation performance.
Visualization: Loss plots provide insights into the training process and model convergence.
Conclusion
The U-Net model for fetal head segmentation demonstrates the effective use of deep learning in medical image analysis. With high accuracy and robustness, this model can assist in automated ultrasound image analysis, contributing to prenatal care and diagnostics.
