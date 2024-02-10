# Student-Summary-Evaluation

# Project Overview:

--> Objective: The project aimed to develop a model to evaluate the quality of summaries written by students in grades 3-12.
--> Data Source: A collection of real student summaries was provided for training the model.
--> Model Selection: DeBERTa-v3-base and BERT-base-uncased models were utilized for their proficiency in understanding contextual information and generating embeddings.
--> Evaluation Metrics: The model assessed the main idea representation, details coherence, and language clarity, precision, and fluency in student summaries.


# Approach Highlights:
1. Utilized DeBERTa-v3-base to predict content and wording RMSE scores, which served as new features for model training.
2. Engineered additional features such as summary-to-context word ratio, cosine similarity, punctuation ratio, similar word ratio, stop word ratio, and word diversity in the student's response.
3. Extracted CLS token embeddings using BERT-base-uncased and selected 10 most important features for modeling.
4. Employed LightGBM boosting method to predict content and wording scores based on the combined features.
