# MATLAB Project: Fruit Classification Using Machine Learning

## Project Description
This project implements a complete fruit classification system using multiple machine learning techniques in MATLAB. It uses image data to train models and classify different fruit types. The dataset includes training, validation, and testing sets, with preprocessing applied to optimize model performance.

## Features
- Image preprocessing and resizing.
- Feature extraction using HOG (Histogram of Oriented Gradients).
- Multiple machine learning models:
  - K-Nearest Neighbors (KNN)
  - Decision Tree (DT)
  - Random Forest (RF)
  - Logistic Regression (with PCA)
  - Convolutional Neural Network (CNN) using ResNet18
- Model evaluation using accuracy metrics.
- Validation set is separated for fine-tuning models.

## Folder Structure
- `/train` - Training dataset organized by fruit class.
- `/val` - Validation dataset organized by fruit class.
- `/test` - Testing dataset organized by fruit class.
- `Matlab.mlx` - Main MATLAB Live Script containing all code (preprocessing, training, evaluation).

## Main Steps
1. **Data Loading:** Import images from train, val, and test folders.
2. **Preprocessing:** Resize images to 128x128 for classic ML models and 224x224x3 for CNN. Apply RGB format for CNN (no grayscale conversion needed for CNN).
3. **Feature Extraction:** Extract HOG features for traditional ML models.
4. **Model Training:** Train various models using the training set.
5. **Model Validation:** Validate models using the validation set.
6. **Testing:** Test the final models and evaluate their performance.
7. **CNN Training:** Modify the final layers of ResNet18 to match the number of fruit classes (37 classes).

## Requirements
- MATLAB R2021a or newer
- Statistics and Machine Learning Toolbox
- Deep Learning Toolbox

## How to Run
1. Clone this repository.
2. Open `Matlab.mlx` in MATLAB.
3. Run each section step-by-step, following the comments.

## Notes
- Make sure to have the correct folder structure with labeled subfolders inside `train`, `val`, and `test`.
- For CNN training, ensure the Deep Learning Toolbox is installed.
- Grayscale conversion is not needed for CNN, images are kept RGB.

## License
This project is for educational purposes only.
