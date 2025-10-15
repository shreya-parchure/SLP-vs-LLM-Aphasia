# Clinician_vs_LLM_Aphasia_Transcription
Code associated with paper "Transformer-based LLM (Whisper) vs Clinician Performance for Transcribing Speech Errors in People with Aphasia"

This repository contains two Python scripts for statistical analysis and visualization of experimental data. The first script (wordFrequencyANOVA.ipynb) performs a one-way ANOVA and Tukey’s HSD post-hoc test to compare error rates across word frequency groups. The second script (linearRegression.ipynb) uses linear regression to examine the relationship between WAB Naming Subscores/WAB AQ and AI hallucination/match rates. Both analyses generate statistical summaries using pandas, scipy, seaborn, and statsmodels.
