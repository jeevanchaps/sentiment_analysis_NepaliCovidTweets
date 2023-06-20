# Sentiment Analysis of Nepali COVID-19 Tweets

This repository contains experiments performed using different monolingual and multilingual Transformer models for the Nepali language to perform the sentiment analysis of the Nepali Tweets related to 
COVID-19. The different monolingual and multilingual models used are as follows which are all available in the HuggingFace.
- [amitness/roberta-base-ne](https://huggingface.co/amitness/roberta-base-ne)
- [Sakonii/distilbert-base-nepali](https://huggingface.co/Sakonii/distilbert-base-nepali)
- [Rajan/NepaliBERT](https://huggingface.co/Rajan/NepaliBERT)
- [bert-base-multilingual-uncased](https://huggingface.co/bert-base-multilingual-uncased)


## DataSets

For this experiment, [NepCOV19Tweets](https://www.kaggle.com/datasets/mathew11111/nepcov19tweets) is used which contains Nepali tweets related to COVID-19.

## Experiments and Results

We experimented with the following:
- Optimizer: AdamW
- Batch Size: 16
- Learning rate: 0.0001

Model Comparsion:

|Model |Pre. |Rec. |F1|
| --- | --- | --- | --- |
|NepaliBERT|0.00| 0.00| 0.00|
|NepBERT|0.00| 0.00 |0.00|
|DB-BERT|0.00 |0.00 |0.00|
|BERT-bbmu|0.00 |0.00 |0.00| 

The results will be updated soon.
