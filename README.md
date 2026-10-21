# Intel Image Classification Using CNN and MobileNetV2

## Project Overview

This project implements an image classification system using a Convolutional Neural Network (CNN) and MobileNetV2 transfer learning. The model classifies natural and urban scene images into six categories using the Intel Image Classification dataset from Kaggle.

The project is developed in Python using TensorFlow and Keras in Google Colab.

## Dataset

**Source:** [Intel Image Classification Dataset — Kaggle](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)

The dataset contains six image categories:

- Buildings
- Forest
- Glacier
- Mountain
- Sea
- Street

The dataset is downloaded programmatically using KaggleHub.

## Technologies Used

- Python
- TensorFlow
- Keras
- MobileNetV2
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- KaggleHub
- Google Colab

## Model Architecture

The project uses MobileNetV2 as a pretrained feature extractor, followed by:

1. Data augmentation
2. MobileNetV2 preprocessing
3. Global Average Pooling
4. Dropout regularization
5. Dense softmax classification layer

The model is trained in two stages: initial training with the pretrained base frozen, followed by fine-tuning selected layers.

## Project Workflow

1. Download the dataset from Kaggle.
2. Locate and load the training and testing folders.
3. Resize images to 160 × 160 pixels.
4. Split training data into training and validation subsets.
5. Apply data augmentation.
6. Train the CNN classification model.
7. Fine-tune selected MobileNetV2 layers.
8. Evaluate the model on the test dataset.
9. Generate accuracy and loss graphs.
10. Create a confusion matrix and classification report.
11. Export predictions and save the trained model.

## Evaluation

The notebook evaluates the model using:

- Test accuracy
- Test loss
- Precision
- Recall
- F1-score
- Confusion matrix
- Actual vs. predicted comparisons

**Results:** Add your actual test accuracy and test loss after running the completed notebook. Results should be reported from the evaluation output rather than estimated.

## Generated Files

- `intel_image_classification_cnn.keras` — trained model
- `intel_cnn_accuracy_loss.png` — training and validation graphs
- `intel_cnn_confusion_matrix.png` — confusion matrix
- `intel_cnn_predictions.csv` — actual and predicted labels with confidence scores
- `intel_cnn_sample_predictions.png` — sample prediction visualization

## How to Run

1. Open Google Colab.
2. Create a new notebook.
3. Copy the project cells into the notebook in order.
4. Run the cells to download the dataset, train the model, evaluate results, and save outputs.
5. Enable a GPU runtime for faster training when available.

## Applications

- Scene image classification
- Computer vision learning
- Transfer learning experiments
- Deep learning model evaluation

## Future Improvements

- Compare different pretrained CNN architectures.
- Tune hyperparameters to improve generalization.
- Analyze class-wise misclassifications.
- Build an interactive image prediction interface.

## Author

**Shafaat Ullah**

AI and Data Science | Machine Learning | Deep Learning

## License

This repository contains project code and documentation. Check the dataset's Kaggle terms and license before redistributing the dataset or its images.
