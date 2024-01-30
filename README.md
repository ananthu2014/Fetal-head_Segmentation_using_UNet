<!DOCTYPE html>
<html>
<head>
    <title>Fetal Head Segmentation Using U-Net</title>
</head>
<body>

<h1>Fetal Head Segmentation Using U-Net</h1>

<h2>Overview</h2>
<p>This project involves the implementation of a U-Net architecture for fetal head segmentation in ultrasound images, using PyTorch. The project showcases the application of deep learning in medical image analysis, particularly in segmenting fetal heads from ultrasound images.</p>

<h2>Key Features</h2>
<ul>
    <li><strong>Technology Stack</strong>: Utilizes libraries like NumPy, PyTorch, OpenCV, PIL, Pandas, and OS.</li>
    <li><strong>Architecture</strong>: The U-Net model comprises 23 convolutional layers, tailored for detailed image segmentation.</li>
    <li><strong>Image Resolution</strong>: Processes images of size 572x572 pixels.</li>
    <li><strong>High Accuracy</strong>: Achieves a Dice score of 95.6% on the test set and a pixel-to-pixel accuracy of 97.4%.</li>
    <li><strong>Hardware Used</strong>: Training and inference performed on an RTX 3080 Ti GPU.</li>
    <li><strong>Data Augmentation</strong>: Includes random rotations, horizontal flips, and vertical flips to enhance model robustness.</li>
    <li><strong>Dataset Size</strong>: Training: 799 images, Validation: 200 images, Testing: 335 images.</li>
    <li><strong>Binary Segmentation</strong>: Predicts binary masks for segmenting the fetal head.</li>
    <li><strong>Loss Plotting</strong>: Visualizes training and validation loss over epochs.</li>
    <li><strong>Early Stopping</strong>: Implements early stopping with checkpoints for saving the best model weights.</li>
</ul>

<h2>Learning Parameters</h2>
<ul>
    <li><strong>Learning Rate</strong>: 0.01</li>
    <li><strong>Batch Size</strong>: 2</li>
</ul>

<h2>Implementation Details</h2>
<ul>
    <li><strong>U-Net Model</strong>: Designed specifically for medical image segmentation. Includes a downsampling and upsampling path.</li>
    <li><strong>Loss Function</strong>: Combines Binary Cross Entropy and Dice Loss.</li>
    <li><strong>Performance Metrics</strong>: Dice score and pixel-to-pixel accuracy.</li>
</ul>

<h2>Usage</h2>
<ol>
    <li><strong>Setup</strong>: Install required Python libraries.</li>
    <li><strong>Data Preparation</strong>: Collect and preprocess ultrasound images.</li>
    <li><strong>Training</strong>: Train the U-Net model on the dataset.</li>
    <li><strong>Evaluation</strong>: Evaluate the model on the test set.</li>
    <li><strong>Inference</strong>: Use the model for segmenting new images.</li>
</ol>

<h2>Additional Information</h2>
<ul>
    <li><strong>Data Augmentation</strong>: Ensures model generalization.</li>
    <li><strong>Early Stopping and Checkpoints</strong>: Prevents overfitting and saves the best model.</li>
    <li><strong>Visualization</strong>: Loss plots provide training insights.</li>
</ul>

<h2>Conclusion</h2>
<p>The U-Net model for fetal head segmentation demonstrates effective use of deep learning in medical image analysis. This model can assist in automated ultrasound image analysis, contributing to prenatal care and diagnostics.</p>

</body>
</html>
