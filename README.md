## VLM – Medical Image Captioning (Work in Progress)

### Overview
- This project explores vision-language models (VLMs) for medical image captioning, with initial experiments using BLIP on the Open-i chest X-ray dataset.
- Current: establishing a baseline, evaluating caption quality, and identifying gaps

### Current Results (BLIP)
- Dataset: Open-i; 2,869 valid image–caption
- Split: Train 2,295 (80%) / Val 287 (10%) / Test 287 (10%)
- Hardware: Used Google Colab
- Training: 10 epochs


### Quantitative Snapshot (20-sample semantic similarity)
- Average similarity: 0.301

#### Strengths
- Learned medical terminology and standard reporting structure
- Good at describing normal findings and producing consistent report-like captions

#### Limitations
- Limited pathological detection 
- Likely chose 'normal' status 
- Overall accuracy is still low

### Planned Improvements
- Improve image augmentation 
- Evaluate alternative/stronger VLM 


