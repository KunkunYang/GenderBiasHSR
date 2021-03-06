## A Causal Inference Method for Reducing Gender Bias in Word Embedding Relations (AAAI 2020)

### Paper
Our paper "A Causal Inference Method for Reducing Gender Bias in Word Embedding Relations" is accepted by AAAI 2020. The arXiv version of this paper (with appendix) is: https://arxiv.org/abs/1911.10787

This repository contains the code of the above paper.

### Download

The Half-Sibling Regression post-processed GloVe embedding (pre-trained on 2017 January dump of English Wikipedia) tested in our paper can be downloaded here: https://drive.google.com/file/d/1w7tl3xSg69L1zURTpQ6qDg0uXab_XKFw/view?usp=sharing

### Instruction

- Please run the file "HSR-GloVe_Gender Direction Relation_&_Lexical- and Sentence-Level Evaluation.ipynb" first to get the post-processed embedding ("hsrglove_wiki_vectors.txt").
- For Gender-Biased Word Relation Task, please first put the original and the post-processed embeddings "glove_wiki_vectors.txt" and "hsrglove_wiki_vectors.txt" into the "Gender-Biased Word Relation Task/source" folder, then run "save_embeds.py" to get the vocabulary and the word vectors. Then, put the vocabulary and the word vector files (txt.vocab and txt.wv.npy) into the folder "Gender-Biased Word Relation Task/data/embeddings", and run "remaining_bias_HSR.ipynb" to get the experimental results of Gender-Biased Word Relation Task.
- Note that the code of Gender-Biased Word Relation Task is written by Gonen and Goldberg 2019 (https://github.com/gonenhila/gender_bias_lipstick), We only made some minor changes such that the code is executable in Python 3.6.
- For the downstream task Gender Coreference Resolution, we utilize the WinoBias dataset (https://github.com/uclanlp/corefBias/tree/master/WinoBias/wino) and the OntoNotes Release 5.0 (https://catalog.ldc.upenn.edu/LDC2013T19). The End-to-end Neural Coreference Resolution model we use in this paper is from this repository by Lee et al. 2017: https://github.com/kentonl/e2e-coref/tree/e2e.


### Requirements
- Environment: Python 3.6 or above
- tensorflow 1.9
- pandas
- gdown
- requests
