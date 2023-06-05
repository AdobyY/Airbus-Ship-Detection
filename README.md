# Airbus Ship Detection

This project focuses on the task of ship detection using semantic segmentation. It uses the U-Net architecture and is trained on the Airbus Ship Detection Challenge dataset from Kaggle.

## Description

The goal of this project is to develop a model capable of accurately segmenting ships in aerial images. Semantic segmentation assigns each pixel in an image to a specific class, enabling pixel-level understanding of the scene. The U-Net architecture, known for its effectiveness in biomedical image segmentation, is employed to achieve this task.

The project includes a Jupyter Notebook (`airbus-ship-detection.ipynb`) that provides the code for training and evaluating the semantic segmentation model. The notebook covers steps such as data preprocessing, model creation, training, and inference on test images. The resulting predicted ship masks are saved in the `submission.csv` file.

## Files Included

- `airbus-ship-detection.ipynb`: Jupyter Notebook containing the code for training and evaluating the semantic segmentation model.
- `requirements.txt`: File listing the required Python packages and their versions for running the project.
- `semantic_segmentation_weights.h5`: Pre-trained weights of the trained semantic segmentation model.
- `submission.csv`: CSV file containing the predicted ship masks for the test images.

## Prerequisites

- Python 3.10
- Tensorflow 2.12
- Other required packages listed in `requirements.txt`

## Installation

1. Clone the repository:

```bash
git clone https://github.com/AdobyY/Airbus-Ship-Detection.git
```

2. Install the required packages:

```bash
pip install -r requirements.txt
```

## Usage

1. Place the training images in the train_v2 folder and the test images in the test_v2 folder.
2. Run the airbus-ship-detection.ipynb Jupyter Notebook to train the semantic segmentation model and generate predictions for the test images.
3. The predicted ship masks will be saved in the submission.csv file.
4. To use the pre-trained weights (semantic_segmentation_weights.h5), load them into your model for ship detection.
