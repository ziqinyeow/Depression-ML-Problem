# Abstract and Introduction

There are 7 notebooks here and each notebook will address different type of problems based on different datasets. Although some datasets are not really reliable, it's worth to try and research. We are approaching this depression detection problem using ensemble technique by combining all the best models trained in each notebooks.

[Notebook 1](#notebook-1) - ML/Structured/Tabular/CSV \
[Notebook 2](#notebook-2) - ML/Structured/Tabular/CSV \
[Notebook 3](#notebook-3) - DL/Unstructured/Image/TIFF \
[Notebook 4](#notebook-4) - DL/Unstructured/Image/PNG \
[Notebook 5](#notebook-5) - DL/Unstructured/Image/PNG \
[Notebook 6](#notebook-6) - DL/Unstructured/Text/CSV \
[Notebook 7](#notebook-7) - DL/Unstructured/Text/CSV \

# Production Deliverables

[Web App](https://deprai.vercel.app/)
[Web GitHub](https://github.com/ziqinyeow/depr.ai)

## Notebook 1 - [Link](./Notebook%201.ipynb)

No implementation yet.

## Notebook 2 - [Link](./Notebook%202.ipynb)

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

Accuracy and time of each model were being compared. \

Data source: [GitHub](https://github.com/patilgirish815/Depression_Detection_Using_Machine_Learning)

## Notebook 3

No implementation yet.

## Notebook 4 - [Link](./Notebook%204.ipynb)

Image binary (2-class) classification problem - Images with 3 color channel (RGB) were trained to perform binary classification on depression and non-depression class.

### Models built - Notebook 4

1. Self-defined CNN (acc: 0.505)
2. Efficient Net Fine Tuned (acc: 0.504)

Data source: [Kaggle](https://www.kaggle.com/datasets/astraszab/facial-expression-dataset-image-folders-fer2013)

Note: Dataset was being classified based on self-experienced (eg: Happy -> Non-depression) but not fully reliable

## Notebook 5

Technique performed and data are the same as [Notebook 4](./Notebook%204.ipynb). The only difference is dataset is not processed based on self-experienced (eg: Happy -> Happy). This notebook more towards emotion classification based on images.

### Models built - Notebook 5

1. Self-defined CNN (acc: 0.3435)
2. Efficient Net Fine Tuned (acc: 0.4648)

## Notebook 6

Text classification (28-class) problem - Text loaded from [Go Emotions](https://huggingface.co/datasets/go_emotions) HuggingFace dataset to fit into a pretrained bert tokenizer and model that classify the text emotion (e.g.: fear, embarrassment, happy...). \

This model is a fine-tuned version of microsoft/xtremedistil-l6-h384-uncased on an unknown dataset. It achieves the following results on the evaluation set: \

Loss: 0.1234 \

Data source: [HuggingFace](https://huggingface.co/datasets/go_emotions)

## Notebook 7

Text classification (2-class) problem - Text loaded from HuggingFace dataset (self-pushed dataset from Kaggle) to fit into a pretrained bert tokenizer and model that classify whether the text is depression or non-depression. \

This model is a fine-tuned version of microsoft/xtremedistil-l6-h384-uncased on an unknown dataset. It achieves the following results on the evaluation set: \

Loss: 0.1606
Accuracy: 0.9565 \

I have push the model to [HuggingFace](https://huggingface.co/ziq/depression_tweet) \

Data Source:

1. [Data 1](https://www.kaggle.com/datasets/gargmanas/sentimental-analysis-for-tweets)
2. [Data 2](https://huggingface.co/datasets/ShreyaR/DepressionDetection/blob/main/depression_dataset_reddit_twitter.csv)
3. [Data 3](https://huggingface.co/datasets/joangaes/depression/blob/main/clean_encoded_df.csv)

Data have been preprocess - [preprocess notebook](./data/Notebook%207%20Data/process.ipynb) and push to [HuggingFace](https://huggingface.co/datasets/ziq/depression_tweet)

# Conclusion

Based on the work done:

1. Tabular - Notebook 1, Notebook 2, Notebook 3
2. Computer Vision - Notebook 4, Notebook 5
3. Natural Language Processing - Notebook 6, Notebook 7

We chose:

1. Notebook 1 - ❌
2. Notebook 2 - model 10
3. Notebook 3 - ❌
4. Notebook 4 - ❌
5. Notebook 5 - ❌
6. Notebook 6 - model 1
7. Notebook 7 - model 1

to build our web application. \

Seem's like some model perform inaccurately especially vision model, we are not going to chose the models to build our web applications. Only tabular and language model will be used in the web application. \

We will be using Next.js and some of the amazing tool to build this web applications. \

[Web App](https://deprai.vercel.app/)
[Web GitHub](https://github.com/ziqinyeow/depr.ai)
