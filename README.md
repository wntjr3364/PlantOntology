# 🌿 POClassifier

**POClassifier: A Transformer-Based Classification Model for Automated [Plant Ontology (PO)](http://www.plantontology.org/) Annotation of NGS Metadata

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

## Overview

**POClassifier** is a deep learning-based classification model for automatically assigning Plant Ontology (PO) terms to unstructured metadata from next-generation sequencing (NGS) datasets. This project was developed to address the challenges of scalable and consistent annotation in plant genomics by leveraging recent advances in natural language processing (NLP), particularly transformer-based models.

## Motivation

The exponential growth of publicly available NGS data has made manual curation of plant-specific metadata increasingly impractical due to its limitations in scalability, reproducibility, and consistency. To support FAIR principles in plant bioinformatics, automated annotation of metadata using standardized ontology terms like PO is essential.


## Features

- ✅ Transformer-based architecture for PO term classification  
- ✅ Trained on augmented datasets generated using large-scale generative language models (e.g., GPT)  
- ✅ Domain-adaptive pretraining using masked language modeling (MLM) on plant-related sequencing metadata  
- ✅ Supports both anatomical entity and developmental stage branches of the Plant Ontology  
- ✅ Compatible with ENA (European Nucleotide Archive) NGS metadata fields


## Data

- **Input**: NGS metadata fields (e.g., `description`, `sample_title`, `tissue_type`)  
- **Labels**: Plant Ontology terms (anatomical entities & developmental stages)  
- **Training Data**:  
  - PO term definitions with GPT-based text augmentation  
  - Real NGS metadata from ENA, curated and preprocessed

## Model Architecture

- Base model: `BERT` or `BioBERT`  
- Fine-tuned on a multilabel classification task  
- Domain-adaptive pretraining: MLM on plant-specific metadata  
- Evaluation metrics: Accuracy, F1-score, Precision, Recall

## Usage

Coming soon — We will provide:

- Inference pipeline with sample metadata input  
- Pretrained weights and tokenizer  
- Command-line usage or notebook-based demo

## Installation

To be updated after model packaging.

## Repository Structure
