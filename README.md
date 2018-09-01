If there is no embedding for a word in the corpus, i.e. the word occurs in the corpus we are looking at but not in the corpus used to generate the embeddings, then it is ignored. We might alternatively use an array of zeros or a unit vector with random direction, but neither contributes to the meaning of the subsequent document embedding. If there is no embedding for any of the words in a document, an array of zeros is taken as its embedding.

I suspect it would be simpler to implement the calculation of the embeddings as a sklearn estimator, but I'm not confident enough to do so at the moment.