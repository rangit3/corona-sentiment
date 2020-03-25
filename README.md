# Fine-grained Sentiment Classification using BERT

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/fine-grained-sentiment-classification-using/sentiment-analysis-on-sst-5-fine-grained)](https://paperswithcode.com/sota/sentiment-analysis-on-sst-5-fine-grained?p=fine-grained-sentiment-classification-using)

This repo contains the code for the kaggle notebook [here](https://www.kaggle.com/ranlevy/how-good-is-a-drug-against-the-corona-virus).

The code is based on the code of the paper [Fine-grained Sentiment Classification using BERT](https://arxiv.org/abs/1910.03474).

## Usage - Inference only. For training use the original repository

Experiments for various configuration can be run using the `run.py`. First of all, install the python packages (preferably in a clean virtualenv): `pip install -r requirements.txt`

```
Usage: run.py [OPTIONS]

  Train BERT sentiment classifier.

  Options:
    -c, --bert-config TEXT  Pretrained BERT configuration
    -b, --binary            Use binary labels, ignore neutrals
    -r, --root              Use only root nodes of SST
    -s, --save              Save the model files after every epoch
    -h, --help              Show this message and exit.
```

For example, to run the experiment for binary labels and root nodes, run:

    python3 run.py -rb

