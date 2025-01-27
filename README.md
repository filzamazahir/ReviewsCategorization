# Reviews Categorization
The purpose of this project is to  develop a system for filtering and categorizing movie reviews. A dataset of IMBD movie reviews with polarity labelling was used to build a model for classifying positive and negative reviews.

## To Run

1) Clone the project
```
git clone https://github.com/filzamazahir/ReviewsCategorization.git
```
Make sure to have pip installed, then do 
```
pip install requirements.txt
```
Run ```reviewscategorization.ipynb```

## Results
Few different models were used to classify the reviews as positive or negative. Model 1, which was Logistic Regression with NLTK and TF-IDF gave the highest F1 score of 0.883 on the test set and passed our criteria, followed by Model 3 which also passed the criteria and gave a F1 score of 0.8775, which used Logistic Regression with spaCy and TF-IDF. LightGBM Classifier with spaCy and TF-IDF gave a F1 score of 0.857 and didn't pass the criteria of F1 score being at least 0.85. All these models did better than a Dummy Classifier which gave a F1 score of 0.335. BERT was not actually run in this project because of the computational power it required, but a BERT text to embeddings function was done still.
