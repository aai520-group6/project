# Final Team Project

## Introduction

This project explores the creation of open source conversational chatbots using transformer networks and transfer learning from pretrained models. We implemented and compared BERT, DistilBERT, and RoBERTa on the Stanford Question Answering Dataset (SQuAD) version 2.

## Models

We leveraged the following pretrained transformer models from HuggingFace:

- [BERT](https://huggingface.co/docs/transformers/model_doc/bert) - Bidirectional Encoder Representations from Transformers
- [DistilBERT](https://huggingface.co/docs/transformers/model_doc/distilbert) - A distilled and smaller version of BERT
- [RoBERTa](https://huggingface.co/docs/transformers/model_doc/roberta) - An optimized method for pretraining BERT models

## Training

The models were fine-tuned on [SQuAD v2](https://rajpurkar.github.io/SQuAD-explorer/) using [Google Colab](https://research.google.com/colaboratory/). We used libraries like HuggingFace [Transformers](https://huggingface.co/docs/transformers/index) and [txtai](https://neuml.github.io/txtai/) to streamline training and evaluation.

## Evaluation

We evaluated using the official [SQuAD v2 validation script](https://worksheets.codalab.org/rest/bundles/0x6b567e1cf2e041ec80d7098f031c5c9e/contents/blob/), which is internally done with HuggingFace's [Evaluate](https://huggingface.co/docs/evaluate/index) library. The evaluation results are published on HuggingFace Model Hub:

- [Fine-Tuned BERT Model](https://huggingface.co/aai520-group6/bert-finetuned-uncased-squad_v2)
- [Fine-Tuned DistilBERT Model](https://huggingface.co/aai520-group6/distilbert-finetuned-uncased-squad_v2)
- [Fine-Tuned RoBERTa Model](https://huggingface.co/aai520-group6/roberta-finetuned-squad_v2)

## Results

- RoBERTa achieved the best performance, highlighting the importance of optimized pretraining.
- All models struggled with unanswerable questions, indicating an area for future work.
- Detailed evaluation results are published on HuggingFace.

## Discussion

The project demonstrates the power of transfer learning for NLP tasks. There is room for improvement in handling unanswerable questions, which is important in preventing hallucinations.
