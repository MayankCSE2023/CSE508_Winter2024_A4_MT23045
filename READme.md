# Problem 1: Data Preprocessing and Model Training

## Approach:

1. **Data Preprocessing:**
   - Loaded the dataset and sampled a smaller subset of rows to reduce computation time.
   - Filtered out rows with missing values.
   - Divided the dataset into training and testing sets.

2. **Model Training:**
   - Utilized the GPT-2 model for text summarization.
   - Implemented a custom dataset class for data loading and tokenization.
   - Fine-tuned the GPT-2 model on the training data using the AdamW optimizer.
   - Trained the model over multiple epochs, monitoring loss and adjusting hyperparameters as needed.

## Methodologies:

- Utilized PyTorch and Hugging Face's Transformers library for model implementation and training.
- Employed AdamW optimizer for optimization during training.
- Implemented custom dataset class and data loader for efficient data processing.
- Utilized tqdm for progress tracking during training.

## Assumptions:

- Assumed that the GPT-2 model is suitable for text summarization tasks.
- Assumed that a smaller subset of the dataset would be representative of the entire dataset.

## Results:

- Successfully trained the GPT-2 model on the sampled dataset.
- Achieved convergence of the training process with acceptable loss values.
- Generated summaries using the fine-tuned model.

---

# Problem 2: Evaluation using ROUGE Scores

## Approach:

1. **ROUGE Scores Calculation:**
   - Evaluated the model's performance using ROUGE scores.
   - Compared the generated summaries with actual summaries from the dataset.
   - Utilized ROUGE metrics (ROUGE-1, ROUGE-2, ROUGE-L) for evaluation.

## Methodologies:

- Used the ROUGE Python package for calculating ROUGE scores.
- Compared generated summaries with actual summaries from the dataset.

## Assumptions:

- Assumed that ROUGE scores provide a reliable evaluation metric for text summarization tasks.

## Results:

- Calculated ROUGE scores for each generated summary compared to actual summaries.
- Evaluated precision, recall, and F1-score for ROUGE-1, ROUGE-2, and ROUGE-L metrics.
- Assessed the model's overall performance based on ROUGE scores.
