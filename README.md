# Clinician_vs_LLM_Aphasia_Transcription
Code associated with paper *Differential Accuracy of Semantic versus Phonological Speech Error Transcription in Aphasia: Comparing Large Language Model (Whisper) to Clinician (SLP) Performance*

Purpose: Patient speech samples provide insights into cognitive and linguistic status, yet their utilization has been limited by labor-intensive manual transcription. Advances in automated speech recognition (ASR) with large language models (LLMs) potentially save time, but performance on impaired speech, such as due to post-stroke aphasia, remains understudied. 

Method: We transcribed 4,535 trials of the Philadelphia Naming Test (PNT) administered to twenty-six people with aphasia (PWA) using OpenAI’s Whisper speech-to-text LLM. These ASR transcripts were compared with gold-standard transcriptions by an experienced speech-language pathologist (SLP). Clinician-LLM match or mismatch in transcription was analyzed across speech-error types (semantic vs phonemic), patient severities, and word frequency.

Results: For each 175-trial PNT, transcriptions by SLP required 180 ± 40 minutes versus 2.3 ± 0.5 minutes by Whisper. Compared to >95% match rate with SLP transcripts for trained humans, Whisper achieved an overall match rate of 75.52%, subdivided as 88.83% match on correct PNT trials, 92.22% on semantic errors, and 23.05% for trials with phonemic errors by PWA. Western Aphasia Battery Aphasia Quotient (WAB-AQ) scores correlated with match rate (R2 = 0.196, p = .023) and hallucination rate (R2 = 0.291, p = .0048). Low-frequency words showed higher mismatch than medium- or high-frequency words (ANOVA F = 14.26, p < .001).

Conclusions: Whisper reliably transcribed semantic but not phonological errors, suggesting automation is best for fluent aphasia types with fewer phonemic distortions. This study benchmarks LLM transcription for impaired speech, offering a scalable alternative to manual transcription that may streamline clinical and research workflows.

---

This repository contains Python scripts for:

1) `Guide: Using Whisper LLM to Transcribe Speech in Aphasia.ipynb` : ASR transcription of speech from people with aphasia (PWA) using Whisper large language model. The python notebook includes tutorial-style comments and simplified code that can run in any browser using Google colaboratory, which includes the optimized settings for anyone to use for speech to text.
2) `wordFrequencyANOVA.ipynb` : Statistical analysis script which contains code used to perform a one-way ANOVA and Tukey’s HSD post-hoc test to compare error rates across word frequency groups.
3) `linearRegression.ipynb` " Visualization of experimental data using code. This script uses linear regression to examine the relationship between WAB Naming Subscores/WAB AQ and AI hallucination/match rates. Both analyses generate statistical summaries using pandas, scipy, seaborn, and statsmodels.
