# Project Design

## Project Overview
Create an AI system to:
- Summarize  news articles into concise summaries.
- Generate Title & Identify Categories (future feature).
- Answer follow-up questions based on the summary (future feature).
The AI will use Hugging Face Transformers with a LLaMA model for text generation.

## 1. Data Collection & Preprocessing
### Data Sources:
Hugging Face datasets & News from internet
### Processing
Tokenize and organize into input-output pairs (full text as input, summary as output).

## 2. Model Selection
Pre-trained Model: Use a LLaMA model (e.g., meta-llama/Llama-3.2-3B-Instruct) for text generation or consider T5/BART for summarization.
Fine-tune the model on the dataset for summarization tasks.

## 3. Model Training
Fine-Tuning:
Fine-tune the datasets from Hugging Face, (abisee/cnn_dailymail)

Save the Model: Store the fine-tuned model locally or upload to Hugging Face Model Hub.

## 4. Evaluation
Metrics: Use ROUGE and BLEU scores to evaluate the summarization quality.
Manual Review: Check generated summaries for quality.

## 5. Deploy
- Gather new data
- Create Interface

