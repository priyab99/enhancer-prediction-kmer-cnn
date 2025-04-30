# Enhancer Prediction using k-mer Features and Multi-Headed CNN

This project predicts DNA enhancer sequences using a deep learning model with four parallel CNN branches, each processing a different k-mer representation (k=1,2,3,4).

## Methodology
- k-mer-based embedding for DNA sequences
- 4-headed CNN with separate convolutional branches
- Trained on 2968 samples, tested on 400 independent sequences
- Ensemble results from 5 cross-validation models

## 📂 Folder Structure
- `src/`: Model and training/testing scripts
- `logs/`: Training logs per fold
- `models/`: Saved best models from 5 folds
- `result/`: Test result


## Experimental Results
All training logs and test results can be found in the `logs/` and `result/`.

## How to Run
```bash
python src/train_enhancer_cnn.py
python src/test_enhancer_cnn.py
