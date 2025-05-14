EastEnders Character Similarity Analysis

This project implements a vector space semantics model to analyze character similarity in the EastEnders script dataset. The goal is to create and refine vector representations of character dialogues from the training data (first 300 lines per character) to distinguish characters based on their spoken lines. The system is evaluated on validation and test datasets (first 50 lines per character) using a similarity-based information retrieval pipeline, aiming to minimize the mean rank metric (target: 1) and improve accuracy.

Project Overview





Dataset: Training (training.csv), validation (val.csv), and test (test.csv) files containing EastEnders script data.



Preprocessing: Enhanced text preprocessing beyond basic tokenization, incorporating at least five techniques to improve text quality and feature extraction.



Feature Extraction: Advanced linguistic feature extraction, including n-grams, POS tags, and TF-IDF transformations, with a minimum of three techniques to enrich vector representations.



Context Incorporation: Integration of dialogue context by including lines from other characters in the same scene, using Episode and Scene metadata (excluding GENDER and CHARACTER columns).



Parameter Optimization: Systematic grid search to tune parameters within preprocessing, feature extraction, and context incorporation stages for optimal performance.



Similarity Analysis: Analysis of character vector similarities using heat map visualizations to identify closest and furthest character matches, with explanations based on linguistic patterns.



Final Evaluation: Testing the optimized system on the test dataset, ensuring proper initialization of transformers and clear reporting of mean rank and accuracy.
