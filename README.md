# Sentiment-Analysis-with-Transformer-Fine-Tuning
This repository contains a Jupyter Notebook implementing sentiment classification on the IMDb dataset using HuggingFace Transformers. It compares full fine-tuning versus LoRA fine-tuning using the peft library to explore the trade-offs in performance and resource efficiency. Notebook includes:
- Dataset preprocessing
- Model training using:
1. Full fine-tuning
2. LoRA (Low-Rank Adaptation) fine-tuning
- Evaluation and comparison
  

**Details**

Method 1: Full Fine-Tuning
The entire model is updated during training. This provides high accuracy but is computationally expensive and memory intensive.

Method 2: LoRA Fine-Tuning (via PEFT)
Uses Low-Rank Adaptation to fine-tune a small subset of parameters. It's resource-efficient and effective for many downstream tasks.


**Evaluation**

The models are evaluated on a subset of the IMDb test set. Metrics include accuracy, training time, and resource usage. Plots and tables are included for comparison.

📎 Dataset
IMDb Movie Reviews: Automatically loaded via datasets.load_dataset('imdb')


**Tools Used**
- HuggingFace Transformers
- PEFT (Parameter-Efficient Fine-Tuning)
- Datasets
- PyTorch, Matplotlib, Pandas
  

**Notes**
- Only a small subset of the dataset is used (3,000 train / 2,000 test) for faster experimentation.
- Code is modular and easy to extend to other models or tasks.
