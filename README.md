<div align="center">

# 🐦 NLP Tweet Classification Challenge

**Irony Detection & Emotion Classification with Transformers**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg)](https://jupyter.org/)
[![HuggingFace](https://img.shields.io/badge/🤗-Transformers-yellow.svg)](https://huggingface.co/)

</div>

---

## 📋 Overview

This repository contains code and datasets for tweet classification across two distinct NLP tasks:

| Task | Type | Classes |
|------|------|---------|
| **Irony Detection** | Binary classification | Ironic / Not Ironic |
| **Emotion Classification** | Multi-class (4) | Anger, Joy, Optimism, Sadness |

## 🧠 Approach

- **Transformer Fine-Tuning** — Pre-trained language models fine-tuned on task-specific tweet datasets
- **Data Augmentation** — Custom augmentation pipeline to handle class imbalance (`data_augmentation_process.ipynb`)
- **Separate Pipelines** — Independent training and inference notebooks for each task

## 📁 Project Structure

```
├── irony_submission.ipynb              # Irony detection pipeline
├── emotion_submission.ipynb            # Emotion classification pipeline
├── data_augmentation_process.ipynb     # Augmentation strategies
├── irony/                              # Irony task data
├── emotion/                            # Emotion task data
├── emotion_train_aug/                  # Augmented emotion training data
└── predictions/                        # Model output predictions
```

## 🚀 Quick Start

1. Set up a Python environment with Jupyter:
```bash
pip install jupyter transformers torch scikit-learn pandas
```

2. Open the notebook for your target task:
```bash
jupyter notebook irony_submission.ipynb
# or
jupyter notebook emotion_submission.ipynb
```

3. Run all cells to train the model and generate predictions.

## 📊 Emotion Label Mapping

| Label | Emotion |
|-------|---------|
| `0` | 😠 Anger |
| `1` | 😊 Joy |
| `2` | 🌟 Optimism |
| `3` | 😢 Sadness |

## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
