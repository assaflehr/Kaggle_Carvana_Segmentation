Code used for the Carvana Image Masking segmentation.

The input is image of a big car on a podium.
The output is segmentation mask of the car vs background. 

Why it's hard?
The leaderboard results were close to 99.5% correct, meaning each pixel matters.
Manual tagging had misses too, and we should match their error types 


Code:
legacy_segmentation_alg.ipynb : trying to immitate the semi-auto manual tagging they used, by running
few legacy edge (sobel) and segmentation algs (wathershed, slic)

unet-kaggle-kernel : modifying open-kernel, to use U-Net