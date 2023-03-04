# Sentiment Classification with Cascade Ensemble Classifier
This project presents a sentiment classification model based on a cascade ensemble classifier. The approach used consists of a two-stage classification process, where the output of the first stage (using a logistic regression classifier) is used as an additional input for the second stage (using a random forest classifier).

## Data Preprocessing
After performing preliminary data cleaning and preprocessing steps, we apply two different word embedding techniques for sentiment analysis classification: Word2Vec and TF-IDF. We evaluate different models for the classification task in both cases.

## Cascade Ensemble Classifier
Our best model, which achieves a F1-score of 0.804, uses a TF-IDF embedding and logistic regression classification model in the first stage. In the second stage, we use the output of the first stage as input for a random forest classifier, along with the date converted to an integer. This approach increases the classification score significantly, resulting in a F1-score of 0.861.

## Conclusion
Our sentiment classification model, based on the cascade ensemble classifier approach, provides an effective solution for sentiment analysis tasks. The combination of TF-IDF embedding, logistic regression, and random forest classifiers results in high accuracy and performance.
