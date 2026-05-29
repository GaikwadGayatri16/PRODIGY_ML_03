# PRODIGY_ML_03

# Cat vs Dog Image Classification using Support Vector Machine (SVM)

## Project Overview

This project implements a Support Vector Machine (SVM) classifier to distinguish between images of cats and dogs. The model uses image preprocessing and Histogram of Oriented Gradients (HOG) feature extraction to convert images into numerical features before classification.

The objective of this project is to demonstrate the application of machine learning and computer vision techniques for image classification.

---

## Internship Task

**Task-03**

Implement a Support Vector Machine (SVM) to classify images of cats and dogs from the Kaggle dataset.

---

## Dataset

Dataset Used: Cats and Dogs Dataset

Dataset Structure:

```text
PetImages/
├── Cat/
│   ├── 0.jpg
│   ├── 1.jpg
│   └── ...
│
└── Dog/
    ├── 0.jpg
    ├── 1.jpg
    └── ...
```

For faster training and experimentation:

- 500 Cat images
- 500 Dog images

Total Images Used:

```text
1000 Images
```

---

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-Learn
- Scikit-Image (HOG)
- Jupyter Notebook

---

## Machine Learning Workflow

### 1. Data Collection

Images of cats and dogs were collected from the dataset.

---

### 2. Image Preprocessing

The following preprocessing steps were applied:

- Convert image to grayscale
- Resize image to 64 × 64 pixels
- Remove invalid images
- Standardize image dimensions

---

### 3. Feature Extraction

Histogram of Oriented Gradients (HOG) was used for feature extraction.

HOG extracts:

- Edge information
- Shape information
- Gradient patterns

This provides more meaningful features compared to raw pixel values.

---

### 4. Train-Test Split

Dataset was divided into:

- 80% Training Data
- 20% Testing Data

Using:

```python
train_test_split()
```

---

### 5. Model Training

Support Vector Machine (SVM) with RBF kernel was used.

Parameters:

```python
SVC(
    kernel='rbf',
    C=10,
    gamma='scale'
)
```

---

### 6. Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Classification Report
- Confusion Matrix

---

## Results

### Model Accuracy

```text
Accuracy: 69%
```

### Classification Report

```text
Precision : 69%
Recall    : 69%
F1-Score  : 69%
```

The use of HOG features improved performance compared to training directly on raw image pixels.

---

## Visualizations

### Sample Images

Displays sample cat and dog images from the dataset.

### Dataset Distribution

Shows the number of cat and dog images used for training.

### Confusion Matrix

Visual representation of classification performance.

### Prediction Results

Displays actual and predicted labels.

### Accuracy Chart

Visual representation of model accuracy.

---

## Project Structure

```text
PRODIGY_ML_03
│
├── PetImages/
│
├── screenshots/
│   ├── sample_images.png
│   ├── dataset_distribution.png
│   ├── confusion_matrix.png
│   ├── accuracy_chart.png
│   └── prediction_results.png
│
├── svm_cat_dog.ipynb
├── svm_cat_dog_model.pkl
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/GaikwadGayatri16/PRODIGY_ML_03.git
```

Move to project directory:

```bash
cd PRODIGY_ML_03
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Required Libraries

```text
numpy
opencv-python
matplotlib
scikit-learn
scikit-image
jupyter
```

Install manually:

```bash
pip install numpy opencv-python matplotlib scikit-learn scikit-image jupyter
```

---

## How to Run

1. Download and extract the dataset.
2. Place the dataset in the project folder.
3. Open the notebook:

```text
svm_cat_dog.ipynb
```

4. Run all cells sequentially.
5. Train the SVM model.
6. Evaluate performance.
7. Visualize predictions.

---

## Applications

This project can be applied in:

- Image Classification
- Computer Vision Systems
- Animal Recognition
- Smart Surveillance Systems
- Automated Image Tagging
- AI-Based Pet Detection

---

## Learning Outcomes

Through this project, the following concepts were learned:

- Image Processing
- Computer Vision
- Feature Extraction using HOG
- Support Vector Machines (SVM)
- Model Evaluation
- Data Visualization
- Machine Learning Workflow

---

## Future Improvements

Possible enhancements:

- Increase training dataset size
- Hyperparameter tuning
- Cross-validation
- Deep Learning using CNN
- Transfer Learning using TensorFlow/PyTorch
- Real-time image prediction application

---

## Conclusion

This project successfully demonstrates the implementation of a Support Vector Machine (SVM) for image classification. Images were preprocessed and transformed into HOG features before training the classifier. The model achieved an accuracy of approximately 69% and successfully classified cat and dog images.

The project highlights the importance of feature extraction in computer vision tasks and provides a practical understanding of image classification using machine learning techniques.

---

## Author

**Gayatri Gaikwad**

Machine Learning Internship Project - Prodigy Infotech

Task-03: Cat vs Dog Image Classification using SVM
