## A Causal Inference Method for Reducing Gender Bias in Word Embedding Relations (AAAI 2020)

### Instruction

- Please run the file "HSR-GloVe_Gender Direction Relation_&_Lexical- and Sentence-Level Evaluation.ipynb" first to get the post-processed embedding ("hsrglove_wiki_vectors.txt").
- For Gender-Biased Word Relation Task, please first put the original and the post-processed embeddings "glove_wiki_vectors.txt" and "hsrglove_wiki_vectors.txt" into the "Gender-Biased Word Relation Task/source" folder, then run "save_embeds.py" to get the vocabulary and the word vectors. Then, put the vocabulary and the word vector files (txt.vocab and txt.wv.npy) into the folder "Gender-Biased Word Relation Task/data/embeddings", and run "remaining_bias_HSR.ipynb" to get the experimental results of Gender-Biased Word Relation Task.
- Note that the code of Gender-Biased Word Relation Task is written by Gonen and Goldberg 2019 (https://github.com/gonenhila/gender_bias_lipstick), We only made some minor changes such that the code is executable in Python 3.6.


### Requirements
- Environment: Python 3.6 or above
- tensorflow 1.9
- pandas
- gdown
- requests
