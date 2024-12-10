# DS 5220 Multiplayer Game Toxicity Detection Using LLMs

This project aims to detect toxic behavior in multiplayer online game chats using advanced language models (LLMs). The primary focus is on identifying the player exhibiting the most toxic traits within a game, based on the entire conversation. The model is fine-tuned to understand the context, tone, and nuances of the chat logs to predict offenders.

## Project Overview

Toxic behavior in online multiplayer games, including harassment, hate speech, and disruptive actions, has become a growing challenge. It impacts player experience, community health, and can even affect a game's financial success. This project explores the use of large language models (LLMs) such as **T5** to detect and identify toxic players based on in-game chat logs.

## Key Features

- **Toxicity Detection:** Identifies players showing toxic behavior in multiplayer games by analyzing chat logs.
- **Context-Aware Models:** Utilizes LLMs (e.g., T5) to understand and process the context of player interactions.
- **Real-Time Prediction:** Designed to process chat logs and predict offenders in real time.
- **Multiple Models:** Compares performance between different LLM models, including **T5**, **DistillBERT**, and **DialoGPT**.

## Experimental Results

- **Main Result:** The final **T5-small** model achieved an accuracy of **36%** for identifying toxic players, which was slightly better than the baseline model but below expectations.
- **Model Comparison:** Although **T5-large** was also tested, the performance was similar to **T5-small**, leading to the decision to continue with the smaller model for computational efficiency.
- **Other Models Tested:** **DistillBERT** and **DialoGPT** were also tried, but they did not perform as well in generating accurate output based on the conversation's context.
- **Training Parameters:** Attempts to adjust **epochs**, **batch size**, and **token size** yielded only a marginal improvement (~1%). Early stopping was used to prevent overfitting, and training was limited to 3 epochs.

## Getting Started

### Prerequisites

To run this project, you will need the following libraries:

- `transformers` (Hugging Face)
- `torch` (PyTorch)
- `pandas`
- `numpy`
- `sklearn`

You can install the required dependencies using:

```bash
pip install -r requirements.txt
```

### Dataset

The dataset used for training and evaluation consists of game chat logs that include:

- **message**: The text message sent by the player.
- **association_to_offender**: Indicates whether the player is the offender, ally, or enemy.
- **case_total_reports**: The number of reports filed for the player.
- **most_common_report_reason**: The main reason for the report (e.g., harassment, negative attitude).
- **chatlog_id**: A unique identifier for each chat log.

## Running the Model

1. Clone the repository
```
git clone https://github.com/ManishKanuri/DS-_5220_FInal_Project_Toxic-behaviour-Detection.git
```
2. Load the dataset

3. Perform Data Cleaning

4. Train the model

5. Evaluate the model

### Hyperparameters
- Learning Rate: 5e-5
- Epochs: 8 (with early stopping)
- Batch Size: 8 (or 16 based on available GPU)
- Tokenizer: T5Tokenizer
- Model: T5ForConditionalGeneration (other models such as DistillBERT and DialoGPT were also tested)

## Limitations
The model's accuracy is still below expectations, and further research is needed to address the task's inherent complexity, such as detecting sarcasm, slang, and non-verbal behaviors.
Performance may vary based on the quality and size of the dataset used for training.
