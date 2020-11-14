# FasterRCNN_AnchorSizeDecay

The success pf custom trained Faster R-CNN networks for image classification will largely depend on the availaility of good & sufficient training data. 

In situations where the training corpous is limited and the training is not progressing well, I noticed that a exponential decay of Anchor Box sizes from the default values to a lesser size is showing promising results. 

Noticed this by pausing the training every n epochs (approx 5000 steps in my case), decreasing Anchor Box sizes (exponential decrease) has given a 10-20% jump in the metrics.
The improvement may be specific to my current project - Hence this approach needs to be studied further in the context of different projects. May be we can create a Custom Anchor_Box_Generator in RPN and experiment.

