# Transfer Learning

A lesson that demonstrates how one may use a pre-trained network requiring enormous computation can be used as the deeper parts of a new network to increase accuracy. These pre-trained networks have essentially extracted most of the low level features and expose them for use. All that is necessary is to train the network built on top of it to extract and combine these features to produce a result.

I can see how this is useful for convolutional neural networks that are great for proximal data (i.e., images), since most networks will need to extract the same features anyways (edges, hue, brightness, noise). But I forsee that this is less suitable for other models (e.g., sequence-to-sequence), as the features extracted may depend heavily on the classification/regression task trained on the network.
