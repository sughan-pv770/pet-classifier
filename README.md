# Pet Classifier

A deep learning model built to classify 37 different breeds of cats and dogs using Transfer Learning with ResNet50.

## Overview

This repository contains a Jupyter Notebook (`pet classifier.ipynb`) that trains a neural network to recognize pet breeds from images. It uses the **Oxford-IIIT Pet Dataset** and leverages a pre-trained **ResNet50** model from TensorFlow/Keras to achieve high accuracy.

## Prerequisites

To run this notebook locally, you will need Python installed along with the following libraries:
- `tensorflow`
- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `jupyter`

You can install them using pip:
```bash
pip install tensorflow numpy pandas matplotlib scikit-learn jupyter
```

## Dataset Setup (Important)

The repository does not contain the images due to their size. You must download the dataset manually and set up the folder structure before running the notebook.

1. **Download the Dataset:**
   Download the Oxford-IIIT Pet Dataset from Kaggle here:
   [The Oxford-IIIT Pet Dataset on Kaggle](https://www.kaggle.com/datasets/tanlikesmath/the-oxfordiiit-pet-dataset)

2. **Organize the Files:**
   - Clone this repository to your local machine.
   - Extract the downloaded dataset.
   - Create a folder named exactly **`images`** in the same directory as the `pet classifier.ipynb` file.
   - Move all the extracted `.jpg` images into this `images` folder.

   Your folder structure should look exactly like this:
   ```text
   pet-classifier/
   │
   ├── pet classifier.ipynb
   ├── README.md
   └── images/
       ├── Abyssinian_1.jpg
       ├── Abyssinian_2.jpg
       ├── american_bulldog_1.jpg
       └── ... (rest of the images)
   ```

## Usage

1. Open a terminal or command prompt in the repository folder.
2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open `pet classifier.ipynb`.
4. Run all the cells sequentially. The notebook will:
   - Load and preprocess the images from the `images` folder.
   - Build a ResNet50-based classification model.
   - Train the model on the images.
   - Plot the training and validation accuracy/loss.
