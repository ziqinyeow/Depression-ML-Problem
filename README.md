# Abstract and Introduction

There are \_ notebooks here and each notebook will address different type of problems based on different datasets. Although some datasets are not really reliable, it's worth to try and research. We are approaching this depression detection problem using ensemble technique by combining all the best models trained in each notebooks.

<a href="#Notebook 1">Notebook 1</a> - ML/Structured/Tabular/CSV</a>
<a href="#Notebook 2">Notebook 2</a> - ML/Structured/Tabular/CSV</a>
<a href="#Notebook 3">Notebook 3</a> - DL/Unstructured/Image/TIFF</a>
<a href="#Notebook 4">Notebook 4</a> - DL/Unstructured/Image/PNG</a>
<a href="#Notebook 5">Notebook 5</a> - DL/Unstructured/Image/PNG</a>

## Notebook 1

## Notebook 2

Tabular 5-class classification problem - 10 questions to classify the person is normal or having mild, moderate, severe or extremely severe depression.

### Steps including

1. Data analysis
2. Feature Engineering
3. Feature Selection
4. Data Preparation
5. Model Experiment
6. Model Evaluation
7. Model Export

### 6 types of model were being built

1. Naive Bayes (acc: 0.8722)
2. K Nearest Neighbour (acc: 0.8983)
3. Support Vector Machine (acc: 0.9576)
4. Decision Tree (acc: 0.8066)
5. Random Forest (acc: 0.9017)
6. Neural Network (acc: 0.9636)

Accuracy and time of each model were being compared. <br />

Data source: <a href="https://github.com/patilgirish815/Depression_Detection_Using_Machine_Learning">GitHub</a>

## Notebook 3

## Notebook 4

Image binary (2-class) classification problem - Images with 3 color channel (RGB) were trained to perform binary classification on depression and non-depression.

### 2 types of model were being built

1. Self-defined CNN (acc: 0.505)
2. Efficient Net Fine Tuned (acc: 0.504)

Data source: <a href="https://www.kaggle.com/datasets/astraszab/facial-expression-dataset-image-folders-fer2013">Kaggle</a>

Note: Dataset was being classified based on self-experienced (eg: Happy -> Non-depression) but not fully reliable

## Notebook 5