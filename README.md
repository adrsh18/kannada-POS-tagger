# ಕಸ್ತೂರಿ (Kasthuri) 
A Parts of Speech tagger for Kannada

##### What was used?
1. Word2Vec to extract features from words
2. Linear Chain CRF to learn tagging rules

**Libraries Used**: gensim, numpy, tensorflow

Sequence of execution:
1. feature-extractor.ipynb - generates feature and label files which may exceed 100 MB.
2. pos-tagger.ipynb - trains on the features and reports performance on test set.

Performance:

|          Class   | precision  | recall | f1-score  | support |
| ---------------- |:----------:|:------:|:---------:|:--------|
|      Conjuncts   |    0.90    |  0.60  |    0.72   |     15  |
|  Demonstrative   |    0.85    |  0.65  |    0.73   |     17  |
|      Adjective   |    0.14    |  0.08  |    0.10   |     49  |
|           Noun   |    0.60    |  0.78  |    0.68   |    306  |
|        Pronoun   |    0.74    |  0.58  |    0.65   |    110  |
|     Adposition   |    0.80    |  0.29  |    0.42   |     14  |
|     Quantifier   |    0.69    |  0.45  |    0.55   |     20  |
|         Adverb   |    0.74    |  0.30  |    0.43   |     46  |
|         Symbol   |    0.99    |  0.99  |    0.99   |     83  |
|      Quotative   |    1.00    |  0.89  |    0.94   |      9  |
|           Verb   |    0.64    |  0.72  |    0.67   |    190  |
