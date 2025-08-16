# ENEM-MIRT-Eval  
**Evaluating Large Language Models on the ENEM using Uni- and Multidimensional IRT**

## Overview  
This repository contains the code, datasets, and experimental results for the paper:  
> *Evaluating Large Language Models through Multidimensional Item Response Theory: A Comprehensive Case Study on ENEM*  
> Leonardo Taschetto, Renato Fileto — Federal University of Santa Catarina  

We present the first application of **Multidimensional Item Response Theory (MIRT)** to evaluate Large Language Models (LLMs) on the Brazilian *Exame Nacional do Ensino Médio* (ENEM), extending beyond raw accuracy to measure **domain-specific proficiencies** on the official human scoring scale.

## Features  
- **Uni-dimensional IRT** replication using INEP’s official 3-PL parameters (2009 baseline).  
- **Four-factor MIRT** model aligned with ENEM’s knowledge domains:  
  - Mathematics (MT)  
  - Natural Sciences (NS)  
  - Human Sciences (HS)  
  - Languages and Codes (LC)  
- Comparison of SOTA LLMs (GPT, DeepSeek, Llama, etc.) across multiple prompting strategies (Few-shot, CoT).  
- Open, reproducible benchmark with calibrated item parameters and evaluation scripts.

## Getting Started  

### Requirements  
- **R >= 4.4.0** with package [`mirt`](https://cran.r-project.org/package=mirt)  
- Python 3.10+ (optional, for preprocessing and evaluation harness)  
- Additional R packages: `tidyverse`, `data.table`  
- Additional Python packages: `pandas`, `numpy`  

### Installation  
Clone the repository:
```bash
git clone https://github.com/leonardotaschetto/enem-mirt-eval.git
cd enem-mirt-eval

