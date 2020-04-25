# pk-batching-for-triplet-loss-tutorial
The concept of triplet loss training is best described in [this blog post by Oliver Moindrot](https://omoindrot.github.io/triplet-loss) and [this tensorflow tutorial](https://www.tensorflow.org/addons/tutorials/losses_triplet) trains a model using it. 

This tutorial is based on [In Defense of the Triplet Loss for Person Re-Identification](https://arxiv.org/pdf/1703.07737.pdf), a paper which shows how to avoid some of the difficulties of triplet loss training. In it they create batches of P classes and K examples from each class to maximise the training speed. 

What I show here is how to create Tensorflow Records with the classes and samples arranged in PK batches so you can optimise your triplet loss training.
