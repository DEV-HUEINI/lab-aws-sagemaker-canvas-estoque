# 📊 Analise de Sentimento em Avaliações de Produtos na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)

Neste Projeto para o Curso de IA do Lab DIO, usei o SageMaker Canvas para criar previsões de Analise de Sentimento em Avaliacao de Produtos com Machine Learning (ML).


## 🎯 Objetivos Deste Desafio de Projeto (Lab)

![image](https://github.com/digitalinnovationone/lab-aws-sagemaker-canvas-estoque/assets/730492/72f5c21f-5562-491e-aa42-2885a3184650)




# Sentiment Analysis of Product Reviews using Amazon AWS SageMaker Canvas

This project demonstrates the use of Amazon AWS SageMaker Canvas to build a machine learning model for sentiment analysis of product reviews. The goal is to analyze customer reviews and determine whether they recommend the products.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Model Building](#model-building)
- [Results](#results)
- [Usage](#usage)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction
Sentiment analysis is a powerful tool used to understand customer opinions and feedback. This project leverages Amazon AWS SageMaker Canvas to create a machine learning model that analyzes product reviews to identify positive or negative sentiments and determine recommendations.

## Dataset
The dataset used in this project consists of product reviews. It includes the following columns:
- `review`: The text of the customer review.
- `recommend`: A binary indicator of whether the customer recommends the product (1 for recommend, 0 for not recommend).

## Data Preparation
Data preparation is a crucial step in building an effective machine learning model. The following steps were taken:
1. **Data Upload**: The dataset was uploaded to Amazon S3.
2. **Data Cleaning**: Removed any unnecessary columns and rows. Only the `review` and `recommend` columns were retained for analysis.
3. **Text Processing**: Performed text preprocessing steps such as tokenization, removal of stop words, and stemming/lemmatization.

## Model Building
Using Amazon SageMaker Canvas, the following steps were followed to build the sentiment analysis model:
1. **Dataset Import**: Imported the cleaned dataset from Amazon S3.
2. **Feature Engineering**: Extracted features from the text data.
3. **Model Training**: Configured and trained the sentiment analysis model using SageMaker Canvas.
4. **Model Evaluation**: Evaluated the model's performance using various metrics like accuracy, precision, recall, and F1-score.

## Results
The model achieved the following performance metrics:
- **Accuracy**: `xx%`
- **Precision**: `xx%`
- **Recall**: `xx%`
- **F1-Score**: `xx%`

## Usage
To use this model:
1. **Clone the Repository**: `git clone https://github.com/your-username/sentiment-analysis-aws-sagemaker.git`
2. **Upload Dataset**: Ensure your dataset is uploaded to Amazon S3.
3. **Run Model**: Follow the instructions in the repository to import the dataset into SageMaker Canvas and run the model.

## Conclusion
This project showcases the power of Amazon AWS SageMaker Canvas in building machine learning models with minimal coding. The sentiment analysis model provides insights into customer reviews and helps in understanding customer satisfaction.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.




