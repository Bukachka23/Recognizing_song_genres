# Music Genre Classification with Support Vector Machine (SVM)

This project demonstrates how to build a music genre classification system using Machine Learning, specifically the Support Vector Machine (SVM) algorithm. The goal is to classify music tracks into three genres: Jazz, Rock, and Classical, based on their audio features.

- Table of Contents
- Introduction
- Prerequisites
- Project Structure
- Data Preparation
- Feature Extraction
- Model Training
- Model Evaluation
- Confusion Matrix
- Usage
- Contributing
- License

## Introduction
Music genre classification is a common problem in the field of audio analysis and machine learning. In this project, we use the MFCC (Mel-Frequency Cepstral Coefficients) feature extraction technique to convert audio tracks into a numerical format that can be used for classification. SVM is chosen as the classification algorithm due to its effectiveness in handling high-dimensional data.

## Prerequisites
Before you begin, make sure you have the following dependencies installed in your Python environment:

- librosa: Used for audio feature extraction.
- numpy: For numerical operations.
- scikit-learn: Provides the SVM classifier.
- matplotlib: Used for data visualization.
- seaborn: For creating a heatmap of the confusion matrix.

You can install these packages using pip:

```
pip install librosa numpy scikit-learn matplotlib seaborn
```

## Project Structure

The project structure is as follows:

```
- /content/drive/MyDrive/Data/genres_original/
  - jazz/
  - rock/
  - classical/
- music_genre_classification.ipynb
- README.md
```

- /content/drive/MyDrive/Data/genres_original/: This directory contains the audio files organized by genre.
- music_genre_classification.ipynb: The Jupyter Notebook containing the code for the project.
- README.md: The documentation you are currently reading.

## Data Preparation
In this section, we specify the directory paths for each genre of music. You should update these paths to match the location of your audio files. The code provided assumes that the audio files are in WAV format.

```
jazz_directory = '/content/drive/MyDrive/Data/genres_original/jazz'
rock_directory = '/content/drive/MyDrive/Data/genres_original/rock'
classical_directory = '/content/drive/MyDrive/Data/genres_original/classical'
```

## Feature Extraction
The extract_features function uses Librosa to extract MFCC features from audio files. MFCCs are commonly used for audio analysis.

## Model Training
We use scikit-learn's SVM classifier (SVC) to train the model. The data is split into training and test sets using train_test_split. The model is then trained on the training data.

## Model Evaluation
We evaluate the accuracy of the trained SVM model on the test data using the model.score function. This accuracy metric gives us an idea of how well the model performs.

## Confusion Matrix
A confusion matrix is generated to visualize the model's performance in classifying each genre. We use matplotlib and seaborn to create a heatmap of the confusion matrix.

## Usage
To run the project:

1. Make sure you have the required dependencies installed.
2. Update the directory paths in the code to point to your own audio files.
3. Execute the Jupyter Notebook music_genre_classification.ipynb.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

##  License
This project is licensed under the MIT License - see the LICENSE file for details.
