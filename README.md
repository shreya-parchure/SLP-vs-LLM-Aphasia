# Clinician_vs_LLM_Aphasia_Transcription
Code associated with paper "Transformer-based LLM (Whisper) vs Clinician Performance for Transcribing Speech Errors in People with Aphasia"

This repository contains Python scripts for:

1) ASR transcription of speech from people with aphasia (PWA) using Whisper large language model. This python notebook includes tutorial-style comments and simplified code that can run in any browser using Google colaboratory, which includes the optimized settings for anyone to use for speech to text.
2) Statistical analysis script `wordFrequencyANOVA.ipynb` which contains code used to perform a one-way ANOVA and Tukey’s HSD post-hoc test to compare error rates across word frequency groups.
3) Visualization of experimental data using code is included in `linearRegression.ipynb`. This script uses linear regression to examine the relationship between WAB Naming Subscores/WAB AQ and AI hallucination/match rates. Both analyses generate statistical summaries using pandas, scipy, seaborn, and statsmodels.
