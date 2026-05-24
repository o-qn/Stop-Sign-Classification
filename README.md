# Traffic Sign Classification using Computer Vision

This repository contains my final assessment project for the Computer Vision course. The objective of this project was to develop a robust, end-to-end Deep Learning pipeline capable of classifying distinct types of traffic signs from image data. 

Everything is self-contained within the `Sign Classification.ipynb` notebook, which walks through data preprocessing, exploratory data analysis, class balancing, model architecture design, training, and detailed evaluation metrics.

## What I Did in This Project

Building an accurate classification model required a heavy emphasis on proper data handling and addressing real-world dataset challenges. The core stages of the project include:

* **Exploratory Data Analysis & Visualization:** Inspected the dataset structures, mapped label indices to actual traffic sign descriptions, and visualized sample images across different classes to understand resolution and lighting variances.
* **Handling Class Imbalance:** Analyzed the distribution of the dataset and implemented targeted data augmentation strategies. This step was crucial to ensure the model didn't heavily favor majority classes and could reliably detect rare traffic signs.
* **Pipeline Customization:** Set up efficient data loaders and split the data into training and validation sets to ensure reliable tracking of generalized performance.
* **Model Training & Evaluation:** Trained a convolutional neural network (CNN) architecture, tracking performance metrics across training epochs to monitor convergence and prevent overfitting.
* **Deep Error Analysis:** Generated a multi-class confusion matrix and a comprehensive classification report (precision, recall, and F1-score per class) to pinpoint exactly which sign types the model confused most frequently.

## Key Insights and Methodology

Traffic sign datasets are notoriously tricky because many signs share similar geometric shapes, color palettes, and internal symbols (such as speed limit signs or various warning symbols). By carefully balancing the dataset upfront and looking closely at per-class precision and recall rather than just overall accuracy, I was able to build a model that handles these fine-grained distinctions much more effectively.

## Want to Run it Yourself?

If you want to play around with the notebook or check out the error analysis, here is how to get set up:

### 1. Grab the dependencies
Make sure you have the standard data science and computer vision libraries installed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```
### 2. Fire up the notebook

Download the repository, make sure your image dataset is structured as expected by the paths in the notebook, and run:
## jupyter notebook "StopSignClassification.ipynb"
