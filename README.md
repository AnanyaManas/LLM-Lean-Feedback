## Overview

This repository contains the experiments performed for the research project at University of Bath.

The project evaluates the efficacy of Large Language Models on mathematical reasoning tasks using 
Lean as a verification and feedback mechanism.

## Abstract of the Project
The integration of Large Language Models (LLMs) with Interactive Theorem Provers (ITPs)
represents a promising direction in mathematical problem-solving. While LLMs can generate
plausible reasoning steps, they lack guarantees of correctness, and are prone to hallucinations.
In contrast, ITPs such as Lean provide rigorous frameworks for mechanically verifying logical
validity. This project investigates the efficacy of combining these systems by leveraging Lean to
provide structured feedback on LLM-generated solutions. Specifically, we evaluate how Lean’s
error messages and verification outcomes can be incorporated into autonomous feedback loops
to guide model performance on mathematical tasks. The goal is to assess whether this hybrid
approach improves the reliability of LLMs in producing correct, machine-verifiable solutions.

## Structure of the Repository
LLM-Lean-Feedback/

│

├── README.md

│

├── data/

│   └── README.md   # explains how to obtain MATH dataset

│

├── problem_1/

│   ├── error_feedback.ipynb
│   ├── binary_correctness.ipynb
│   ├── logs/
│   │   ├── build_log_1.docx
│   │   ├── build_log_2.docx
│   │   └── build_log_3.docx
│   └── output/
│
├── problem_2/
│   ├── code.ipynb
│   └── results.docx
│
├── problem_3/
│   ├── test_1/
│   │   ├── code.ipynb
│   │   └── logs/   # 1000 CSVs
│   └── test_2/
│       ├── code.ipynb
│       └── logs/   # 165 files
│
└── dissertation/
    └── dissertation.pdf

## Dataset
The MATH dataset (Hendrycks et al) is not included due to licensing restrictions.

## Requirements
- Python 3.x
- Lean 4 + mathlib
- Jupyter Notebook
