# LLM-Enhanced-Iterative-Framework
We introduce an iterative modular code generation framework that systematically decomposes tasks into smaller subtasks, generates code chunks based on these subtasks, and iteratively improves these code chunks. The final product is then evaluated and integrated into a cohesive whole. Our framework leverages Retrieval-Augmented Generation (RAG) for code generation, improves code quality through iterative improvements, and combines LLM with control flow graph (CFG) analysis for evaluation.

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

## Description

- **generate_framework_Core** contains the main function definition functions of the three parts of the framework: Planning, Iterative Improvement, and Quality Evaluation, but does not include import and main calling functions
(The complete code for this project will be provided upon acceptance of the associated research paper.)
- **generate_direct** directly uses LLMs to generate code
- **all-MiniLM-L6-v2** local version of the embedding model (or all-MiniLM-L6-v2 of Hugging Face)
- **README** provides an overview of installation, usage instructions, and project structure.
- **dataset_vectorization**Import APPS dataset and build vector database
