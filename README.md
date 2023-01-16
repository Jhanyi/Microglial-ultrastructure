# Microglial ultrastructure
Source code for generating a raw features database from segmentation data <br>
Microglial segmentation was performed with [VAST lite](https://lichtman.rc.fas.harvard.edu/vast/) and exported as tiff files. <br>

## Files
### For generation of raw features
Cells.py generates index labels from tiled binary images containing whole-cell segmentations and creates bounding boxes <br>
MGFeatures.py contains tools to extract raw features like "area" (i.e. number of pixels) and "ER lengths" (i.e. [Open CV arc length](https://docs.opencv.org/4.x/dd/d49/tutorial_py_contour_features.html)) <br>
See Usage - get features.ipynb for how this is implemented
featuresraw_v05.xlsx is the result of the implementation

### For comparing with manually classified cells.
compare_manual.ipynb matches manually classiified cells with blindly segmented cells to a common index
