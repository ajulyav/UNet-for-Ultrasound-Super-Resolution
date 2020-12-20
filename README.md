# UNet-for-Ultrasound-Super-Resolution
UNet Architecture for Medical Ultrasound Image Super-Resolution

The baseline UNet network is developed for the problem of super-resolution of ultrasound medical images (L1 pixel-wise loss).

The feature of this network is its symmetry and the idea of re-usability of the data from middle to the up-convolution layers. The left side is the contracting path which is responsible for feature extractions, while the right side called the expansive path - for decoding.

In context of solving the SISR problem, one of the most applied losses are pixel-wise which compute the error between the ground truth image (high-resolution) and recovered one (super-resolution). Recent approaches prefer using mean absolute error due to its more robustness. Thus, L1 is used to train this network.
