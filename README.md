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
	1.	Clone the repository:
    ```{bash}
    git clone https://github.com/your-username/piqa-evaluation.git
cd piqa-evaluation
    ```
    2.	Install the required Python libraries:
    ```{bash}
        pip install -r requirements.txt
    ```
    The requirements include:
	•	transformers
	•	datasets
	•	torch
	•	matplotlib (optional, for visualization)
## Usage
	1.	Run the Evaluation Script:
Use the provided script to evaluate the models:
```{bash}
python evaluate_models.py
```
	2.	Customize Evaluation:
	•	Modify the max_examples parameter in the code to evaluate on more examples.
	•	Add other pre-trained models for comparison.
## Results
The results of the evaluation on 20 examples from the PIQA validation set are as follows:
```{bash}
| Model               | Accuracy (%) |
|---------------------|--------------|
| facebook/opt-1.3b   | 70.00        |
| roberta-large-mnli  | 55.00        |

```
## Citations

	•	PIQA Dataset: https://huggingface.co/datasets/piqa
	•	Hugging Face Transformers: https://github.com/huggingface/transformers
	•	Hugging Face Datasets: https://github.com/huggingface/datasets
	•	Meta OPT Model: https://huggingface.co/facebook/opt-1.3b