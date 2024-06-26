Subtheme Sentiments Analysis-:

Overview-:
The objective of this project is to identify sub-themes and their respective sentiments in given text samples, such as reviews.

Approach
Data Exploration
The initial dataset comprised around 10,000 data points with approximately 90 unique labels. After preprocessing and addressing label frequency issues, we reduced the data to 6,000 points with 23 unique labels. Detailed exploration can be found in the Data Exploration document.

Model Selection
This task is treated as a multi-label classification problem. We used pre-trained BERT models, fine-tuning them to fit our data. BERT was chosen for its effectiveness in handling language models and its ease of implementation.

Pre-trained Models Used:
bert-base-uncased
bert-large-uncased
For simplicity and efficiency, the bert-base-uncased model was selected despite bert-large-uncased performing slightly better. The model can be downloaded from this link.

Training Details
We used Binary Cross Entropy with Logits as the loss function. The model was trained for 5 epochs before overfitting was observed. More details are available in the Model Analysis document.

Performance Metrics
Micro F1 Score: Reflects overall performance, particularly useful for imbalanced classes.
Macro F1 Score: Calculates the mean of F1 scores for each label, not accounting for label imbalance.
Hamming Loss: Measures the fraction of incorrect labels.
