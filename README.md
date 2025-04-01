# Corrective Context Generation for Misleading News Headlines

This repository contains code for a project that detects misleading news headlines and generates corrective context to clarify them. The current work includes data exploration and baseline experiments for both classification and generation tasks. The project is a grad project for the course INFO 259 at UC Berkeley with Prof. David Bamman.

## Overview

- **Detection**: A baseline binary classifier (using features like TF-IDF and sentiment scores) distinguishes misleading headlines from reliable ones.
- **Generation**: A baseline summarization module (leveraging pre-trained models such as BART, T5, or pointer-generator networks) produces concise corrective summaries from full articles.

## Repository Structure

- **data/**: Contains datasets
- **notebooks/**: Contains preprocessing, exploration and baseline scripts
- **reports/**: Contains the reports for my class INFO 259

## Getting Started

1. **Clone Repository**  
   ```bash
   git clone https://github.com/row56/headlinecontext.git
   cd headlinecontext

2. **Install Dependencies**  
   ```bash
    pip install -r requirements.txt

3. **Run Baselines**  
    - Data exploration: data_exploration.ipynb
    - Classification baseline: classification_baseline.ipynb
    - Generation baseline: generation_baseline.ipynb

## Experiments & Evaluation

Classification: Experiments on the LIAR and Clickbait datasets using a logistic regression model.
Generation: Summarization experiments evaluated with ROUGE scores on a subset of the Newsroom dataset.

## Upcoming Additions

Throughout the project, additional enhancements will be implemented, including:

- Integration: Combining the detection and generation modules into a unified, end-to-end pipeline
- Refinement: Further fine-tuning of the classification and summarization models based on extensive experiments
- Extended Evaluation: Incorporating human evaluations alongside automatic metrics like ROUGE and BERTScore
- Distant Supervision: Exploring distant and weak supervision techniques to improve training on limited labeled data
- (Limited) Scalability: Optimizing the pipeline to handle larger datasets and real-world news articles
- Documentation: Regular updates to code documentation and experimental results to ensure reproducibility

## Report

For further details on the project refer to the reports.
