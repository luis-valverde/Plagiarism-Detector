# Plagiarism Detector

## Table Of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Neccessary Files](#neccessary-files)
- [How to Run](#how-to-run)

## Introduction

This repository contains all my work for the Udacity's Machine Learning Nanodegree Program.

The goal in this project was to build a plagiarism detector to clasify text files as either plagiarized or not depending
on how similar it is to a provided source text.

To accomplish this, I defined features for comparing the similarity of an answer text and a source text, and selected
features by analyzing the correlations between them. Then, created a binary classification model, trained and deployed
it using Amazon SageMaker. Finally, I calculated the accuracy of the final model (obtained 0.960 accuracy).

## Project Overview

Plagiarim is when you copy/paste and present someone else's work as it was your own, that's considered stealing of
intellectual properties.

In this project, you will be tasked with building a plagiarism detector that examines a text file and performs binary
classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a
provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences
between paraphrased answers and original work are often not so obvious.

This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**:

1. Load in the corpus of plagiarism text data.
2. Explore the existing data features and the data distribution.
3. This first notebook is **not** required in your final project submission.

**Notebook 2: Feature Engineering**:

1. Clean and pre-process the text data.
2. Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
3. Select "good" features, by analyzing the correlations between different features.
4. Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Your Model in SageMaker**:

1. Upload your train/test feature data to S3.
2. Define a binary classification model and a training script.
3. Train your model and deploy it using SageMaker.
4. Evaluate your deployed classifier.

## Requirements

This project uses the following software and Python libraries:

- [Python](https://www.python.org/downloads/release/python-364/)
- [NumPy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [scikit-learn (v0.17)](https://scikit-learn.org/0.17/install.html)
- [Matplotlib](https://matplotlib.org/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html).

If you do not have Python installed yet, it is highly recommended that you install the
[Anaconda](https://www.anaconda.com/distribution/) distribution of Python, which already has the above packages and
more included.

## Neccessary Files

This repository contains three files needed to solve the project.

1. **1_Data_Exploration.ipynb:** Explore the existing data features and the data distribution.
2. **2_Plagiarism_Feature_Engineering.ipynb:** Clean and pre-process the text data.
3. **3_Training_a_Model.ipynb:** Train and test your model and deploy it using SageMaker.
4. **helpers.py:** Utilities functions to use in the project.
5. **problem_unittests.py:** Unit tests to verify correct functionality of the algorithms created.
6. **source_sklearn:** Hold starting code for a custom Scikit-learn model.
7. **source_pytorch:** Hold starting code for a custom PyTorch model.

## How to Run

In the Terminal or Command Prompt, navigate to the folder on your machine where you've put the project files, and then
use the command:

```bash
jupyter notebook 2_Plagiarism_Feature_Engineering.ipynb
```

 to open up a browser window or tab to work with your notebook.
 Alternatively, you can use the command:

 ```bash
jupyter notebook
```

or

```bash
ipython notebook
```

and navigate to the notebook file (2_Plagiarism_Feature_Engineering.ipynb) in the browser window that opens.
