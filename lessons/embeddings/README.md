# Word Embeddings with Word2Vec

A lesson on generating word embeddings using a Skip-gram Word2Vec model.

Word embeddings are words encoded as vectors such that vectors close to each other contain similar semantic meaning. Word2Vec is a collection of models used to generate word embeddings by training neural networks on a corpus and using the resulting weight matrix in the hidden layer as a lookup table for each word token. Skip-gram is one such model architecture that is trained to predict the context `C` given a word `W` (`P(C|W)`). Word2Vec can be thought of as a way to compress the vector space of independent words (one-hot unit vectors means that any two words are equidistant from each other) into much fewer dimensions by clustering similar terms together (Note that "similar" in this context refers to distributional semantics, i.e., a word's meaning is influenced by the words it is surrounded by).

I can see how this could be useful in trying to determine what someone intends to do given a sentence. Sometimes a user may not say something correctly, but can still be understood via their semantic meaning (e.g., non-native speaker). Word2Vec could help by calculating the intention from vector representations of each word to carry forward the semantic meaning without being hampered by specific words that may be slightly off in meaning.
