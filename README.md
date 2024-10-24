# ResumAI ("resume" + "AI")

## About
ResumAI is a An intelligent resume screening and ranking system powered by Large Language Models. ResumAI uses fine-tuned Mistral-7B with a mathematical weighted scoring algorithm as an apporach to evaluate and rank resumes against job descriptions.

## Overview
This repository contains the implementation of the paper "AI-Driven Recruitment: A Novel Framework for Automating Resume Screening and Ranking using Large Language Models". The work introduces a methodology for creating realistic synthetic datasets that pair job descriptions with corresponding resumes, along with a weighted mathematical model for resume scoring.

## Key Features
- 🤖 Fine-tuned LLM for accurate resume analysis
- 📊 Weighted Mathematical scoring system that mimics human evaluation
- 🎯 Precise matching between job requirements and candidate profiles
- 💼 Comprehensive evaluation of experience, skills, and qualifications
- ⚡ Efficient PEFT/LoRA implementation for optimal performance
- 📝 Detailed explanations for each resume score

## Contents

1. **Synthetic Dataset Creation**:  
   This notebook (`synthetic_dataset_creation.ipynb`) contains all the code related to generating the synthetic dataset used for fine-tuning the models. I implemented a step-by-step procedure as described in the [methodology shared in the PDF](https://drive.google.com/file/d/1Y4gk-bRUmloiVAqDgQuGS8e-qpkfikx2/view).

2. **Fine-Tuning LLaMA2**:  
   The notebook (`finetuning_llama2.ipynb`) includes code for fine-tuning the LLaMA2 model on the synthetic dataset, as well as the results obtained. The code covers pre-processing, training, evaluation, and saving the fine-tuned model.

3. **Fine-Tuning Mistral7B**:  
   Similarly, the notebook (`finetuning_mistral7b.ipynb`) provides the entire process for fine-tuning the Mistral7B model on the same dataset. Results, comparisons, and insights are documented at the end of this notebook.

4. **Research Paper**:  
   You can access the full research paper outlining the approach, methodology, experiments, and results in greater detail through [this link](https://drive.google.com/file/d/1Y4gk-bRUmloiVAqDgQuGS8e-qpkfikx2/view).

## Datasets

The training and testing datasets for the instruction-tuning experiments have been uploaded to Hugging Face. You can find them here:

- [Hugging Face Dataset: Mistral7B Instruction Tuning](https://huggingface.co/datasets/shyamshanckin6/mistral7B-instruction-resume/settings)  
  Dataset repository: `shyamshanckin6/mistral7B-instruction-resume`

This dataset includes the instruction-tuned training and test datasets used for both the LLaMA2 and Mistral7B models.

