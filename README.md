# LLM-Enhanced-Iterative-Framework
An LLM-enhanced Iterative Framework for Modular Code Generation in Complex Tasks

## Project Overview

This project evaluates the framework for solving encoding problems for large language models such as GPT-4, DeepSeek-V2.5, and GLM-4-Plus using the APPS dataset.

## Datasets

- **APPS dataset**: A collection of real encoding problems

## Models

- **Base language models:**
- GPT-4
- DeepSeek-V2.5
- GLM-4-Plus
- ...

- **Embedding model:**
- all-MiniLM-L6-v2 from Hugging Face for the vector database.

## Settings

- **Strategy:** Each subtask is iterated for a maximum of 5 times, and the evaluation feedback iteration lasts for a maximum of 5 rounds
- **Temperature:** Set to 1.0
- **Maximum output length:** is 4000 tokens

## Settings and Installation

1. Download all-MiniLM-L6-v2 and place it in the corresponding location（or all-MiniLM-L6-v2 of Hugging Face ）
2. Use generate_framework.ipynb and follow the prompts to install the corresponding package
