# Abstract and Introduction

There are eight notebooks here, and each notebook will address different types of problems based on different datasets. Although some datasets are not really reliable, it's worth trying and researching. For example, we approach this depression detection problem using the ensemble technique by combining all the best models trained in each notebook.

[Notebook 1](#notebook-1---link--) - ML/Structured/Tabular/CSV \
[Notebook 2](#notebook-2---link--) - ML/Structured/Tabular/CSV \
[Notebook 3](#notebook-3) - DL/Unstructured/Image/TIFF \
[Notebook 4](#notebook-4---link-) - DL/Unstructured/Image/PNG \
[Notebook 5](#notebook-5---link-) - DL/Unstructured/Image/PNG \
[Notebook 6](#notebook-6---link-) - DL/Unstructured/Text/CSV \
[Notebook 7](#notebook-7---link-) - DL/Unstructured/Text/CSV \
[Notebook 8](#notebook-8---link-) - DL/Unstructured/Text/CSV

# Production Deliverables

[Web App](https://deprai.vercel.app/) \
[Web GitHub](https://github.com/ziqinyeow/depr.ai)

## Notebook 1 - [Link](./Notebook%201.ipynb) <img align="right" src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"> <img align="right" src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">

Tabular 5-class classification problem - 10 questions to classify the person is normal or having mild, moderate, severe or extremely severe depression.

### Steps including

1. Data analysis
2. Feature Engineering
3. Feature Selection
4. Data Preparation
5. Model Experiment
6. Model Evaluation
7. Model Export

### 6 types of models were being built

1. Naive Bayes (acc: 0.8722)
2. K Nearest Neighbour (acc: 0.8983)
3. Support Vector Machine (acc: 0.9576)
4. Decision Tree (acc: 0.8066)
5. Random Forest (acc: 0.9017)
6. Neural Network (acc: 0.9636)

The accuracy and time of each model were compared.

Data source: [GitHub](https://github.com/patilgirish815/Depression_Detection_Using_Machine_Learning)

## Notebook 2 - [Link](./Notebook%202.ipynb) <img align="right" src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"> <img align="right" src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">

Tabular 2-class classification problem - 30 questions to classify the person is depression or non-depression.

### 1 type of model was being built

1. Neural Network (acc: 0.893)

Data source: [GitHub](https://github.com/Sabab31/Depression-Repository/blob/main/Depression%20Dataset.csv)

## Notebook 3 - [Link](./Notebook%203.ipynb)

No implementation yet.

The JAFFE dataset consists of 213 images of different facial expressions from 10 different Japanese female subjects. Each subject was asked to do 7 facial expressions (6 basic facial expressions and neutral) and the images were annotated with average semantic ratings on each facial expression by 60 annotators.

Data source: [JAFFE](https://www.v7labs.com/open-datasets/jaffe#:~:text=The%20JAFFE%20dataset%20consists%20of,facial%20expression%20by%2060%20annotators.)

## Notebook 4 - [Link](./Notebook%204.ipynb) <img align="right" src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">

Image binary (2-class) classification problem - Images with 3 color channels (RGB) were trained to perform binary classification on depression and non-depression classes.

### Models built - Notebook 4

1. Self-defined CNN (acc: 0.505)
2. Efficient Net Fine Tuned (acc: 0.504)

Data source: [Kaggle](https://www.kaggle.com/datasets/astraszab/facial-expression-dataset-image-folders-fer2013)

Note: Dataset was being classified based on self-experienced (eg: Happy -> Non-depression) but not fully reliable

## Notebook 5 - [Link](./Notebook%201.ipynb) <img align="right" src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white">

The technique performed and data are the same as [Notebook 4](./Notebook%204.ipynb). The only difference is dataset is not processed based on self-experienced (eg: Happy -> Happy). This notebook is more towards emotion classification based on images.

### Models built - Notebook 5

1. Self-defined CNN (acc: 0.3435)
2. Efficient Net Fine Tuned (acc: 0.4648)

## Notebook 6 - [Link](./Notebook%206.ipynb) <img align="right" src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white">

Text classification (28-class) problem - Text loaded from [Go Emotions](https://huggingface.co/datasets/go_emotions) HuggingFace dataset to fit into a pretrained Bert tokenizer and model that classify the text emotion (e.g.: fear, embarrassment, happy...).

This model is a fine-tuned version of microsoft/xtremedistil-l6-h384-uncased on an unknown dataset. It achieves the following results on the evaluation set:

Loss: 0.1234

Data source: [HuggingFace](https://huggingface.co/datasets/go_emotions)

## Notebook 7 - [Link](./Notebook%207.ipynb) <img align="right" src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white">

Text classification (2-class) problem - Text loaded from HuggingFace dataset (self-pushed dataset from Kaggle) to fit into a pretrained Bert tokenizer and model that classify whether the text is depression or non-depression. \

This model is a fine-tuned version of microsoft/xtremedistil-l6-h384-uncased on an unknown dataset. It achieves the following results on the evaluation set:

Loss: 0.1606

Accuracy: 0.9565

I have pushed the model to [HuggingFace](https://huggingface.co/ziq/depression_tweet)

Data Source:

1. [Data 1](https://www.kaggle.com/datasets/gargmanas/sentimental-analysis-for-tweets)
2. [Data 2](https://huggingface.co/datasets/ShreyaR/DepressionDetection/blob/main/depression_dataset_reddit_twitter.csv)
3. [Data 3](https://huggingface.co/datasets/joangaes/depression/blob/main/clean_encoded_df.csv)

Data have been preprocess - [preprocess notebook](./data/Notebook%207%20Data/process.ipynb) and push to [HuggingFace](https://huggingface.co/datasets/ziq/depression_tweet)

## Notebook 8 - [Link](./Notebook%208.ipynb) <img align="right" src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=PyTorch&logoColor=white">

Unsupervised representational text generation problem - Approximately 100 rows of texts were collected from multiple [data source](./data/Notebook%208%20Data/README.md). Fine-tune a pretrained Distilled GPT2 model from HuggingFace.

This model is a fine-tuned version of distilgpt2. It achieves the following results on the evaluation set:

Loss: 3.3740

This model couldn't be exported after several trials. So we decided to train a model pipeline to be able to generate 1000 suggestions and save them to a CSV file.

Generated Suggestions: [See Generated Text](./data/Notebook%208%20Data/generated_suggestions.csv)

The model was pushed to [HuggingFace Hub](https://huggingface.co/ziq/depression_suggestion)

Data source: [GitHub](./data/Notebook%208%20Data/README.md)

Data have been preprocess - [preprocess notebook](./data/Notebook%208%20Data/process.ipynb) and push to [HuggingFace Hub](https://huggingface.co/datasets/ziq/depression_advice)

# Conclusion

Based on the work done:

1. Tabular - Notebook 1, Notebook 2, Notebook 3
2. Computer Vision - Notebook 4, Notebook 5
3. Natural Language Processing - Notebook 6, Notebook 7

We chose:

1. Notebook 1 - model 10
2. Notebook 2 - model 1
3. Notebook 3 - ❌
4. Notebook 4 - ❌
5. Notebook 5 - ❌
6. Notebook 6 - model 1
7. Notebook 7 - model 1
8. Notebook 8 - generated_suggestions (1000 records)

to build our web application.

Seem's like some models perform inaccurately, especially vision models; we are not going to choose the models to build our web applications. So only tabular and language model will be used in the web application.

We will be using Next.js and some of the amazing tools to build the web application.

[Web App](https://deprai.vercel.app/) \
[Web GitHub](https://github.com/ziqinyeow/depr.ai)

# Reference

[https://www.mayoclinic.org/diseases-conditions/depression/diagnosis-treatment/drc-20356013](https://www.mayoclinic.org/diseases-conditions/depression/diagnosis-treatment/drc-20356013)
