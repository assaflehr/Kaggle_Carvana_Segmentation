Code used for the Carvana Image Masking segmentation.


Input: Image of a big car on a podium in the middle of the image.
Output:segmentation mask of the car vs background. 

Simple, ain't it? using a semantic segmentation network , like UNet should solve it.
Why it's hard to win?
* The leaderboard results were close to 99.5% correct, meaning each pixel really matters, and your results should be beyond State-of-the-art on this task.
* You have to work with full image resolution and a (very) strong GPU. 
* The ground-truth mask was done in a semi-automatic tool. If you can replicate it, it can help to tune for replicating the errors.


Code:
unet-kaggle-kernel : modifying open-kernel, to use U-Net
legacy_segmentation_alg.ipynb : trying to immitate the semi-auto manual tagging they used, by running few legacy edge (sobel) and segmentation algs (wathershed, slic). 

