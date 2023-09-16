# next-word-prediction-using-BiLSTM
1. The program read a file containing an english story.
2. It then removes pucntuation from the story and tokenizes the story.
3. It then generates ngrams (n is a configurable parameter).
4. For each ngram, the first n-1 words of will be used as x-set and the last word will be used as label.
5. The words in x-set are converted into word embeddings using google word2vec model.
6. The words in y-set are converted into one-hot encoding. The size of each one-hot encoding is equal to the size of vocabulary.
7. The model is then trained using 32 as batch size and 100 as number of epochs.
