Toxic Player Detection Using Sentiment Analysis and Random Forest Model
This project demonstrates the implementation of a machine learning model for detecting toxic players in multiplayer games based on their chat logs. The model uses sentiment analysis (via VADER) and a Random Forest Classifier to identify whether a player is an offender or not based on their chat behavior. The dataset required for this project is expected to be uploaded by the user.

Overview
The objective of this project is to detect toxic players in a game based on their chat logs. The model processes the chat messages, analyzes sentiment, and identifies players who exhibit toxic behavior. The primary task is to classify players as offenders (toxic) or non-offenders based on the sentiment of their messages.

Features
Data Cleaning and Preprocessing: Handles missing values, filters relevant game logs, and assigns player IDs.
Sentiment Analysis: Analyzes the sentiment of chat messages using the VADER sentiment analyzer.
Offender Identification: Classifies players based on the sentiment of their chat logs, labeling offenders with a score above a certain threshold.
Model Training: Uses a Random Forest Classifier to predict offenders.
Evaluation: Evaluates model performance using F1 Score, Confusion Matrix, and Classification Report.
Setup
Prerequisites
A Google account to use Google Colab.
The chatlogs.csv file containing the chat log data.
Python libraries:
pandas
scikit-learn
vaderSentiment
numpy
Steps to Run
Clone this repository or download the .ipynb file to your system.

bash
Copy code
git clone <repository-url>
Open the Toxic_Player_Detection.ipynb file in Google Colab.

Upload the chatlogs.csv file:

Place the file in the specified path /content/chatlogs.csv as expected by the notebook.
Alternatively, modify the file path in the notebook to match your file location.
Run the notebook cells sequentially to process the data, build the model, and generate results.

Files
Toxic_Player_Detection.ipynb: The Jupyter Notebook containing the code for the project.
chatlogs.csv: The input dataset (to be uploaded by the user). This file should contain chat logs from games.
Results
The notebook will output:

Predicted offenders for each game.
A list of flagged players along with their champion names and sentiment scores.
Evaluation metrics (F1 Score, Confusion Matrix, Classification Report).
Zero-Tolerance Sentiment Threshold
This model uses sentiment analysis to identify toxic behavior. The sentiment score is computed using the VADER sentiment analyzer, which assigns a "compound" score to each message. The following thresholds are used:

A positive sentiment score indicates a non-offender (label 0).
A negative sentiment score indicates a potential offender (label 1), based on the score falling below a set threshold.
The sentiment threshold for labeling an offender can be adjusted within the notebook.

Sentiment Words List
The sentiment analysis model (VADER) does not use a predefined dictionary of toxic words but instead evaluates the sentiment polarity of entire chat messages. VADER's dictionary includes words with emotional content that are relevant for detecting negative behavior in chat logs. Some example words contributing to sentiment scores include:

Negative words: "hate", "stupid", "idiot", "trash", "noob".
Positive words: "good", "great", "friendly", "positive".
Model Evaluation
The model’s performance is evaluated based on:

F1 Score: Measures the balance between precision and recall.
Confusion Matrix: Shows the number of true positives, false positives, true negatives, and false negatives.
Classification Report: Provides precision, recall, and F1-score for each class (offender and non-offender).
Conclusion
This project provides a framework for identifying toxic players in multiplayer game chat logs. By utilizing sentiment analysis and machine learning, it classifies players as offenders based on their chat messages. You can easily extend or modify the model for further improvements, such as incorporating additional features or experimenting with different machine learning models.

