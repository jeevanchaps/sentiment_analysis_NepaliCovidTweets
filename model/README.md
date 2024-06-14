

# Model Card for Model ID

This model was developed by finetuning the [DistilBERT Nepali Model](https://huggingface.co/Sakonii/distilbert-base-nepali). The model classifies the Nepali tweets related to COVID19 into three categories: neutral, positive and negative.



- **Developed by:** Jeevan
- **Model type:** DistilBERT Nepali
- **Language(s) (NLP):** Nepali
- **Finetuned from model [optional]:** [DistilBERT Nepali Model](https://huggingface.co/Sakonii/distilbert-base-nepali)



## Training Details

### Training Data

The dataset used for finetuning this model can be found at [NepCOV19Tweets](https://www.kaggle.com/datasets/mathew11111/nepcov19tweets) which contains Nepali tweets related to COVID-19.

### Training HyperParameters 

* Batch size: 16
* Learning Rate: 0.0001
* Optimizer: AdamW
* Epochs: 10



## Evaluation

* Training loss: 0.2414
* Precision: 0.73
* Recall: 0.73
* F1 Score (Weighted): 0.73

## Labels

* Neutral: 0
* Positive: 1
* Negative: 2


## USAGE

```python
from transformers import pipeline

pipe = pipeline("text-classification", model="xap/Sentiment_Analysis_NepaliCovidTweets")
pipe("अमेरिकामा कोभिड बाट एकै दिन चार हजारभन्दा बढीको मृत्यु")
```

## Citation

```
@misc {jeevan_2024,
	author       = { {jeevan} },
	title        = { Sentiment_Analysis_NepaliCovidTweets (Revision 3086409) },
	year         = 2024,
	url          = { https://huggingface.co/xap/Sentiment_Analysis_NepaliCovidTweets },
	doi          = { 10.57967/hf/2243 },
	publisher    = { Hugging Face }
}
```
