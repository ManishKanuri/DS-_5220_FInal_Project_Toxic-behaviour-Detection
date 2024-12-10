
# Traditional Zero-Tolerance Word-Based Model

This project demonstrates the implementation of a **Traditional Zero-Tolerance Word-Based Model** for identifying toxic players in chat logs. The model is built using Python and runs seamlessly on **Google Colab**. The dataset required for this project is expected to be uploaded by the user.

## Overview

The objective of this project is to detect toxic players in a game based on their chat logs. The model uses a dictionary of predefined "zero-tolerance" words/phrases to flag players based on their chat content. It identifies the player with the highest count of toxic words in each game as the predicted offender.

## Features

- **Data Cleaning and Preprocessing**: Handles missing values, aggregates messages, and assigns player IDs.
- **Zero-Tolerance Dictionary**: Matches chat messages against a comprehensive list of predefined toxic words.
- **Offender Identification**: Flags the player with the highest toxic word count for each game.
- **Evaluation**: Compares the predicted offenders with actual offenders (if labeled data is available).

## Setup

### Prerequisites

- A Google account to use **Google Colab**.
- The `chats.csv` file containing the chat log data.

### Steps to Run

1. Clone this repository or download the `.ipynb` file to your system.
   ```bash
   git clone <repository-url>
   ```

2. Open the `Traditional__model_.ipynb` file in **Google Colab**.

3. Upload the `chats.csv` file:
   - Place the file in the specified path `/content/chats.csv` as expected by the notebook.
   - Alternatively, modify the file path in the notebook to match your file location.

4. Run the notebook cells sequentially to process the data, build the model, and generate results.

## Files

- `Traditional__model_.ipynb`: The Jupyter Notebook containing the code for the project.
- `chats.csv`: The input dataset (to be uploaded by the user).

## Results

The notebook will output:
- Predicted offenders for each game.
- A list of flagged players along with their champion names and toxic word counts.
- Evaluation metrics (accuracy, if actual labels are available).

## Zero-Tolerance Word List

The model uses a comprehensive dictionary of toxic words and phrases such as:
`"noob", "trash", "report", "idiot", "stupid", "hate", "kill", "moron", "afk", "feed", "toxic", "inting", "grief", "loser", "kys", "troll"`, and many more.

This list can be customized within the notebook.


