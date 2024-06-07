# CMU Wearable Healthcare Technology course project (2021)

## Aim
We aim to develop an image analysis and machine learning pipeline for automated detection of sweat rate and chloride concentration from sweat patches, using smartphone-based images of the patch. 

### Content details and Pipeline
1. Capture photo
2. Match sweat patch photo to template photo (using template matching algorithms)
3. Apply affine transform on sweat patch image to standardize the image
4. Segment out sweat patch channels
5. Compute contour-based area of segmented color channels.
6. Sweat rate and Cl concentration is estimated from contour-based area using a pre-calibrated and trained regression model.

The regression model mentioned above is trained with known ground truth numbers and with similar pre-processing of images
