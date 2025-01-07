# CIFAR-10 Classification with PyTorch

This project involves training a Convolutional Neural Network (CNN) on the CIFAR-10 dataset using PyTorch. The goal was to practice my data science and deep learning skills, ensuring they remain sharp. It covers loading, transforming, and normalizing data, defining a simple CNN model, training the model, and evaluating its performance.

---

## Steps Implemented

### 1. Dataset Loading and Preprocessing
- Used the CIFAR-10 dataset, which consists of 60,000 images in 10 classes (e.g., airplanes, cars, etc.).
- Preprocessed the data by:
  - Converting images to tensors.
  - Normalizing them to have a mean of `0.5` and a standard deviation of `0.5` for all three RGB channels.

### 2. Model Architecture
Defined a simple CNN model with:
- **2 Convolutional Layers**: Extract spatial features.
- **MaxPooling Layers**: Downsample feature maps to reduce dimensionality.
- **Fully Connected Layers**: Perform final classification with 10 output classes.

### 3. Training
- Trained the model for 30 epochs using:
  - **CrossEntropyLoss**: To calculate the classification error.
  - **SGD Optimizer**: Learning rate set to `0.001` with momentum of `0.9`.
- Logged the loss during training. For example:
  - After 10 epochs: Loss = `1.073`
  - After 30 epochs: Loss = `0.528`

### 4. Evaluation
- Tested the model on the CIFAR-10 test dataset.
- Achieved **64.65% accuracy** after 30 epochs.

---

## Key Insights
- The model showed steady improvement with reduced loss and improved accuracy.
- Despite the relatively simple CNN architecture, the results demonstrated that the model learned meaningful patterns from the CIFAR-10 dataset.
- Identified potential areas for improvement, including:
  - Adding data augmentation for better generalization.
  - Increasing network depth or using pretrained models like ResNet.
  - Using advanced optimizers (e.g., Adam) and learning rate schedulers.

---

## Technologies Used
- **Python**: Main programming language.
- **PyTorch**: For building, training, and evaluating the CNN.
- **Google Colab**: For training the model in a cloud-based environment.

---

## Future Improvements
- Experiment with more advanced architectures (e.g., ResNet18 or VGG).
- Add regularization techniques like dropout.
- Incorporate data augmentation for more robust training.
- Fine-tune hyperparameters and experiment with different optimizers.

---

This project was a great hands-on exercise to revisit key data science and deep learning concepts. The practical implementation keeps my skills sharp and ready for application to more advanced challenges.
