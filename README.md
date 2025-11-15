# Multi-Modal Meme Classification Model | Summer Internship @ NIT

Developed a state-of-the-art multi-modal deep learning model that classifies sentiment from internet memes by jointly analyzing textual and visual content.

## Tech Stack
- **Framework**: PyTorch
- **Transformers**: XLM-RoBERTa, CLIP
- **Attention**: Multi-Head Attention
- **Libraries**: Transformers, OpenCV

## Table of Contents
- [Architecture](#architecture)
- [Results](#results)

---

## Architecture

&lt;div align="center"&gt;
  &lt;img src="MODEL_01.png" alt="Model Architecture" style="background-color: white; padding: 15px; border-radius: 8px; max-width: 100%;"&gt;
&lt;/div&gt;

### Methodology
1. **Feature Extraction**:
   - Fine-tuned XLM-RoBERTa → 768-d text features from OCR text
   - Fine-tuned CLIP → 512-d text features + 512-d image features

2. **Fusion**: Concatenated to obtain 1792-d unified representation

3. **Attention**: Processed through multi-head attention transformer

4. **Output**: Binary sentiment classification

---

## Results

&lt;div align="center"&gt;
  &lt;img src="Screenshot%202025-11-16%20013649.png" alt="Results Visualization" style="background-color: white; padding: 10px; border-radius: 6px; max-width: 100%;"&gt;
&lt;/div&gt;

### Performance Metrics
| Metric | Score |
|--------|-------|
| **Weighted F1** | **0.6882** |
| **ROC-AUC** | **0.71** |

*Surpasses state-of-the-art benchmarks on meme sentiment classification.*

---

**Repository**: `Multi-modal-Meme-Classification-Model--Summer-Intern-NIT`
