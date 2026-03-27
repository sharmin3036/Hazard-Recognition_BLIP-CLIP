# Automated Construction Hazard Recognition and Captioning with Contrastive Language Image Pre-training (CLIP) and Bootstrapping Language Image Pre-training (BLIP) Vision-Language Models: Does Prompt Engineering Improve Precision?
---

## Overview  

This repository contains the code for our study on **automated construction hazard recognition using Vision-Language Models (VLMs)**. The project evaluates **CLIP and BLIP-2** for multi-label hazard detection using **zero-shot, prompt engineering, and few-shot learning strategies**.  

---

## Models  

| Model | Type | Description |
|------|------|------------|
| **CLIP (ViT-B/16)** | Pretrained | Contrastive vision-language model using image-text similarity |
| **BLIP-2 OPT-2.7B** | Pretrained | Vision-language model for VQA |
| **BLIP-2 FLAN-T5-XL** | Pretrained | Instruction-tuned VLM for improved reasoning and prompt sensitivity |

---

## Repository Structure  

```
Hazard-Recognition_BLIP-CLIP/
├── data/
├── models/
├── scripts/
├── utils/
├── configs/
├── results/
├── requirements.txt
└── README.md
```

---

## Setup  

```
git clone https://github.com/sharmin3036/Hazard-Recognition_BLIP-CLIP.git
cd Hazard-Recognition_BLIP-CLIP
pip install -r requirements.txt
```

---

## Dataset  
The dataset is a curated subset of a construction safety dataset (Roboflow), reformulated for image-level multi-label classification with the following classes:
- Helmet (Hardhat)  
- Safety Vest  
- Safety Cone  
- Machinery  
- Vehicle

## Experiments

### Phase 1: Zero-Shot Baseline
- CLIP → Descriptive prompts  
- BLIP-2 → Binary VQA prompts  

---

### Phase 2: Prompt Engineering
Evaluate three prompt styles:
- Direct  
- Contextual  
- Safety Compliance  

---

### Phase 3: Few-Shot Learning
Caption-guided few-shot prompting using exemplar Q&A pairs.


## 📈 Key Results  

| Model | Baseline F1 | Best Prompt F1 |
|------|------------|---------------|
| CLIP | 0.44 | 0.53 |
| BLIP-2 OPT | 0.38 | 0.39 |
| BLIP-2 FLAN | 0.37 | 0.52 |

## 📄 Related Publication

**Automated Construction Hazard Recognition and Captioning  
With Contrastive Language Image Pre-training (CLIP) and Bootstrapping Language Image Pre-training (BLIP) Vision-Language Models (VLMs): Does Prompt Engineering Improve Precision?**

*Sharmin Jahan Badhan and Reihaneh Samsami*  
ASCE International Conference on Computing in Civil Engineering (i3CE), 2026

This study explores the use of vision-language models (VLMs), including CLIP and BLIP, for automated hazard recognition and captioning in construction environments. The research evaluates the impact of prompt engineering on model precision, contributing to safer and more intelligent construction inspection workflows.


## Authors
- Sharmin Jahan Badhan
- Reihaneh Samsami
```
