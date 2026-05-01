# 🐦 NLP Tweet Classification Challenge

NLP project for tweet classification on two tasks:

1. **Irony detection** (binary)
2. **Emotion classification** (4 classes)

## 🧠 Labels

Emotion mapping:

- `0`: Anger
- `1`: Joy
- `2`: Optimism
- `3`: Sadness

## ⚙️ Approach

- Transformer fine-tuning for both tasks
- Data augmentation pipeline for class balancing (`data_augmentation_process.ipynb`)
- Separate notebooks for each submission workflow

## 📁 Main Files

- `irony_submission.ipynb`
- `emotion_submission.ipynb`
- `data_augmentation_process.ipynb`
- `irony/`, `emotion/`, and `predictions/` folders

## 🚀 How to use

1. Prepare your Python/Jupyter environment
2. Open the notebook for the target task
3. Run training + inference cells
4. Export predictions in the required challenge format

