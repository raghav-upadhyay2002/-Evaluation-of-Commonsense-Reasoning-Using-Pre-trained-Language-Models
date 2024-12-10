# Evaluation of Commonsense Reasoning Using Pre-trained Language Models
This repository contains the code and resources for evaluating the zero-shot performance of two pre-trained large language models (LLMs) on the Physical Interaction Question Answering (PIQA) dataset. The goal is to assess the ability of LLMs to reason about physical scenarios without additional fine-tuning.
## Overview
This project compares the performance of two models:
	1.	facebook/opt-1.3b: A general-purpose pre-trained model from Meta.
	2.	roberta-large-mnli: A model fine-tuned for natural language inference (NLI) tasks.

The evaluation uses a subset of the PIQA validation dataset to measure the accuracy of these models in predicting the most plausible solution for physical commonsense reasoning tasks.

## Features
	•	Dataset: Integration with the PIQA dataset using Hugging Face Datasets.
	•	Models: Zero-shot evaluation of pre-trained models (facebook/opt-1.3b and roberta-large-mnli).
	•	Evaluation: Custom function for calculating model accuracy.
	•	Comparison: Results highlight the strengths and weaknesses of each model.

## Setup
    ### Prerequisites
  	•	Python 3.7 or higher
	•	pip package manager
    ### Installation