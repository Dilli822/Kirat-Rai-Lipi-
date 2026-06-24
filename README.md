# KIRAT RAI LIPI CHARACTER RECOGNITION AND PRESERVATION USING LIGHTWEIGHT PRETRAINED MODELS FOR EDGE DEVICE BENCHMARKING

The Kirat community is an indigenous group of eastern Nepal with a rich linguistic heritage, including Kirat Rai languages and their writing systems. Many of these languages are increasingly under-documented and are experiencing rapid decline in intergenerational transmission, making them vulnerable to long-term loss. This highlights the need for computational approaches to support their preservation and accessibility. In this work, we focus on the digital preservation of Kirat Rai Lipi through AI-based character recognition. We introduce the first curated and annotated dataset of Kirat Rai Lipi characters for low-resource script modeling. To establish a baseline, we fine-tune and evaluate multiple pretrained deep learning vision models, including efficient transformer-based architectures optimized for low-latency inference on edge devices. Experimental results demonstrate strong performance in character classification, achieving competitive accuracy and F1-scores under limited data conditions. To the best of our knowledge, this is the first study to develop a dedicated Kirat Rai Lipi dataset and evaluate pretrained models for its recognition, enabling future real-time digitization and multimodal language processing systems. Our code is available at:[github.com/Dilli822/Kirat-Rai-Lipi-](https://github.com/Dilli822/Kirat-Rai-Lipi-) 

---

## Table of Contents

* [Kirat Rai Lipi](https://claude.ai/chat/481d6645-3219-4b25-b773-c89b24dd1d20#kirat-rai-lipi)
* [Overview](https://claude.ai/chat/481d6645-3219-4b25-b773-c89b24dd1d20#overview)
* [Models Evaluated](https://claude.ai/chat/481d6645-3219-4b25-b773-c89b24dd1d20#models-evaluated)
* [Results](https://claude.ai/chat/481d6645-3219-4b25-b773-c89b24dd1d20#results)
* [Cite This Work](https://claude.ai/chat/481d6645-3219-4b25-b773-c89b24dd1d20#cite-this-work)
* [License](https://claude.ai/chat/481d6645-3219-4b25-b773-c89b24dd1d20#license)

---

## Kirat Rai Lipi

<p align="center">
  <img src="Kirat Rai LIPI IMG/kiratrai.jpg" alt="Kirat Rai Lipi Script" width="480"/>
</p>
Kirat Rai Lipi is the indigenous writing system of the Rai community, one of the Kirat peoples of Nepal and Northeast India. The script is used to write the Rai languages and carries deep cultural and historical significance. This project aims to digitize and recognize Kirat Rai Lipi characters using modern lightweight deep learning models, contributing to the preservation and computational representation of this endangered script.

---

## Overview

This project benchmarks ten lightweight pretrained models on a custom Kirat Rai Lipi character classification dataset. Models are fine-tuned using a frozen backbone strategy (head-only training) and evaluated on Top-1 accuracy, Top-5 accuracy, Precision, Recall, and F1 score.

---

## Models Evaluated

| Model                | Trainable Params |
| -------------------- | ---------------- |
| EfficientFormerV2-S0 | 1.34M            |
| EdgeNeXt-XX-Small    | 0.88M            |
| FastViT-T8           | 2.90M            |
| EfficientFormer-L1   | 9.08M            |
| TinyViT-5M           | 3.15M            |
| MobileNetV4-Small    | 1.27M            |
| MobileOne-S1         | 0.04M            |
| TinyNet-E            | 0.24M            |
| EfficientViT-M0      | 0.17M            |
| ViT-Small DINOv3     | 14.19M           |

---

## Results (mean ± std over 2 seeds)

| Model                | Top-1 Acc (%) | Top-5 Acc (%)  |
| -------------------- | ------------- | -------------- |
| EdgeNeXt-XX-Small    | 99.40 ± 0.00 | 100.00 ± 0.00 |
| EfficientFormerV2-S0 | 98.79 ± 0.60 | 100.00 ± 0.00 |
| FastViT-T8           | 98.49 ± 0.90 | 100.00 ± 0.00 |
| EfficientFormer-L1   | 97.29 ± 0.30 | 100.00 ± 0.00 |
| TinyViT-5M           | 96.69 ± 0.30 | 100.00 ± 0.00 |
| MobileNetV4-Small    | 69.28 ± 1.20 | 91.57 ± 0.60  |
| MobileOne-S1         | 66.57 ± 3.92 | 90.96 ± 1.81  |
| TinyNet-E            | 61.75 ± 0.90 | 87.05 ± 0.30  |
| EfficientViT-M0      | 59.04 ± 1.21 | 90.06 ± 0.90  |
| ViT-Small DINOv3     | 24.40 ± 1.38 | 61.15 ± 7.53  |

---

## Usage

Google Colab Notebook: [www.kaggle.com/code/dillihangrai078/kirat-rai-lipi-recognition-computer-vision-ai](https://www.kaggle.com/code/dillihangrai078/kirat-rai-lipi-recognition-computer-vision-ai)

---

## Cite This Work

If you use this work, dataset, or code in your research, please cite:

```bibtex
@article{PLACEHOLDER_KEY,
  author    = {Last, First and Last, First and Last, First},
  title     = {Your Paper Title Here},
  journal   = {Journal or Conference Name},
  year      = {202X},
  volume    = {XX},
  pages     = {XX--XX},
  doi       = {10.XXXX/XXXXXXX},
  url       = {https://doi.org/10.XXXX/XXXXXXX}
}
```

> **How to export:**
> Copy the BibTeX block above and paste it into your `.bib` reference file.
> Most reference managers (Zotero, Mendeley, JabRef) support direct BibTeX import via  **File → Import** .

---

## License

This project is for research purposes only.
