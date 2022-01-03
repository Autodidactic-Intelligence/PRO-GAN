# PRO-GAN
A progressively growing GAN built using the Keras API.

The PRO-GAN is built following the paper Progressive Growing of GANS for Improved Quality, Stability, and Variation by Tero Karras, Timo Aila, Samuli Laine, and Jaakko Lehtinen. This is complete with the alpha weighting layers to smoothly integrate new blocks into the model along with pixel normalization. When adding another block to the model the old alpha layers are removed by specifically indexing their position in the model, this could likely be done more elegantly but works as is.

The program is split into two parts, one for originally creating the network, start, and one for continuing the progress, continue, trained to  an output resolution of 128x128.
