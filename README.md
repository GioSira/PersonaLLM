# Large Language Model Persona Impact Evaluation

## Project Overview

This project aims to evaluate the impact of integrating various personas into a Large Language Model (LLM) for Natural Language Processing (NLP) tasks. 
By feeding the LLM with predefined personas, we assess how effectively it can adopt these characters to perform specific tasks. 
The central hypothesis is that the LLM, when provided with a persona context, will deliver responses that align better with the given persona's characteristics, potentially improving task performance.

## Datasets Used

### Summarization Task Dataset

For the summarization task, we utilized **CNN/Dailymail** dataset for text summarization. 
The dataset contains a collection of news article from the DailyMail and CNN website. 
The published articles in those sites comprises stories and associated highlights that serve as summaries.

### Hellaswag

We employed the **Hellaswag** dataset, which is designed to test the model's understanding of natural language through multiple-choice questions. 
Each instance requires the model to choose the most appropriate ending to a given context, making it an excellent measure of the model's narrative understanding and reasoning.

## Folder Structure and Scripts

The project repository is divided into specific folders, each containing scripts relevant to the different parts of the project:

### cnn_dm Folder

This directory contains scripts related to the DailyMail and CNN datasets for summarization tasks:

- **cnn_dm_prompt_creator.py**: This script generates prompts that are used to instruct the LLM to summarize articles from the DailyMail and CNN datasets.

- **cnn_dm_evaluation.py**: After the LLM generates summaries, this script evaluates the performance of the model against the gold standard summaries provided in the datasets.

### hellaswag Folder

This directory includes scripts for the Hellaswag dataset related to the NLU task:

- **create_hellaswag_examples.py**: It creates a subset of examples from the Hellaswag dataset to be used for prompt generation.

- **hellaswag_prompt_creator.py**: This script produces prompts that guide the LLM to complete sentences based on the provided context and endings in the Hellaswag dataset.

- **hellaswag_evaluation.py**: Following the LLM's attempts to solve the Hellaswag tasks, this script is used to assess its accuracy and measure the influence of the personas on the model's performance.

## Conclusion

By conducting this project, we aim to shed light on the potential of persona-based modifications to enhance the performance of Large Language Models in NLP tasks. 
The scripts and datasets form a comprehensive test bed for analyzing the effects of such modifications and contribute to the growing field of personalized AI interactions.
