# Intro to Recurrent Neural Networks

A lesson on how Recurrent Neural Networks work. RNNs use controlled feedback loops in their neurons to allow the network to keep track of previous inputs, i.e., it gives them memory of sequences seen in the past and uses that information to weigh in on the output. These are especially useful for language modelling, since languages consist of sequences of characters over an alphabet.

For me, this lesson was much more difficult to understand conceptually than the previous lessons on Convolutional Neural Networks and densely connected Neural Networks. There's this LSTM black box (I'm sure subsequent lessons will cover it) that can be unpacked so that it may be differentiable. Then the network itself operates on sequences, outputting the next character in the batch, which adds another dimension to the inputs (creating a 3d tensor), then weighted by a final output layer to produce a softmax one-hot encoding of the alphabet. The character with the highest probability wins.

It's qute mind-boggling how RNNs can generate entirely new character sequences that look very similar to what it was trained on. It is able to understand that words are separated by spaces, vowel/consonant placement, word sequences, and pick up on some basic grammar. Very cool to see in action.
