# colorize-restoreimages
Colorize and restore old black &amp; white images

### This repo will house code/learning to colorize and restore old, destoyed and black & white images

## Final Version has four components.
We split the network into encoder and decoder. Between them we'll use a fusion layer. In parallel to the encoder, the input images also run through inception resnet v2. ***We extract the classification layer and merge it with the ouptut from the encoder.***

By transferring the learning from the classifier to the coloring network, the network can get a sense of what's in the picture. Thus, enabling the network to match an object representation with a coloring scheme.