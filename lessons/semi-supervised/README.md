# Semi-supervised Learning

A lesson on semi-supervised learning with GANs, in which there are only a small subset of labeled data points that a classifier can train on. Instead of focusing on generating data modelling the source distribution (G), we can instead focus on the discriminator (D) to learn how to classify from both labeled and unlabeled data. This trains a classifier that usually has a higher accuracy than if it was just trained on the labelled examples.

The intuitive idea is that by showing the classifier some more unlabelled examples, it is able to extract features better so that it best models the real examples, and not noise from those examples. The classifier combines what it knows about its labelled data with what it knows about what data is fake or not to produce a more accurate representation for solving the classification problem.
