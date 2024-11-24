
# Fine-Tuning and Evaluating BERT on SQuAD 2

This repository demonstrates how to fine-tune and evaluate a BERT model for a Question Answering (QA) task using the **SQuAD 2.0** dataset. The project includes scripts for both fine-tuning and evaluation.

---

## Project Structure

- **`QA_SQUAD2_BERT_base_Fine-tuning.ipynb`**: Jupyter notebook for fine-tuning the BERT base model on the SQuAD 2.0 dataset.
- **`QA_SQUAD2_BERT_base_Evaluation.ipynb`**: Jupyter notebook for evaluating the fine-tuned BERT model on the validation dataset.

---

## Dataset

- **SQuAD 2.0** (Stanford Question Answering Dataset): 
  - Includes over 100,000 questions and corresponding context paragraphs.
  - Features unanswerable questions, adding complexity to the QA task.

---

## Steps to Run

### 1. Fine-Tuning
1. **Install Dependencies**:
   ```bash
   pip install datasets transformers
   ```
2. **Run the Notebook**: Open and execute `QA_SQUAD2_BERT_base_Fine-tuning.ipynb`.
3. **Key Components**:
   - Loading the dataset using `datasets` library.
   - Tokenizing inputs with `transformers.AutoTokenizer`.
   - Fine-tuning the BERT model using PyTorch.

### 2. Evaluation
1. **Upload the Fine-Tuned Model**:
   - The evaluation notebook requires the fine-tuned model saved from the fine-tuning process.
2. **Run the Notebook**: Open and execute `QA_SQUAD2_BERT_base_Evaluation.ipynb`.
3. **Key Metrics**:
   - Exact Match (EM)
   - F1 Score

---

## Dependencies

Install the required libraries:
```bash
pip install datasets transformers torch tqdm
```

---

## Results

- The fine-tuned BERT model is evaluated on the SQuAD 2.0 validation dataset.
- Outputs include:
  - Exact Match (EM) score.
  - F1 score to measure overall model performance.

---


## Author

Created by **dim_k**.
