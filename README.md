# [Medical Image Captioning with BLIP](https://kensuke-blog-website-1759988624.s3.us-east-1.amazonaws.com/projects/blip_medical_results.html)
*Faster radiology reporting through automated image captioning*

## Project Overview

For a summary and results, please visit the [dedicated project page](https://kensuke-blog-website-1759988624.s3.us-east-1.amazonaws.com/projects/blip_medical_results.html).

- Vision–Language Model project focused on medical image captioning for chest X-rays, using BLIP as the baseline.
- Goal: Assess feasibility for clinical-style reporting, identify gaps for pathology coverage.

## Why healthcare

- Medical imaging reports must be precise, safe, and aligned with clinical language. This project emphasizes:
- Data ethics and safety guardrails for non-diagnostic usage
- Transparent reporting of limitations and error modes

## Dataset and Setup

- Dataset: Open-i chest X-ray (paired images and reports)
- Preprocessing: Standard resize/normalization
- Split: Train 2,295 (80%) / Val 287 (10%) / Test 287 (10%) out of 2,869 valid pairs
- Training: 10 epochs 

## Current Results (BLIP baseline)
- 20-sample semantic similarity: 0.301

### Observed strengths

- Captures standard reporting structure and medical terminology
- Produces consistent, report-like captions for normal or near-normal findings

### Limitations

- Tends toward "normal" summaries
- Accuracy is limited without domain-specific fine-tuning and evaluation. Also the dataset is pretty small and need more computing power to implement in a larger scale


## Further Improvement

- Improve data augmentation and regularization
- Human-in-the-loop error analysis for pathology-specific failure modes