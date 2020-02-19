# CropVigorIndex

CVI is a derived multi-spectral index for usage with the KolariVision Infrared Blue/NIR NDVI filter (and similar). It is intended to closely parallel the values of leaf-level NDVI (e.g. GreenSeeker), though it currently does not occupy the same domain of values.

CVI has seen numerous revisions, each with the intent of improving the detection of Crop Vigor, especially against bare soil.

# Comparison of methods

The below methods assume that a typical tri-band visible sensor (RGB) is being used with a full-spectrum conversion alongside the application of either an internal or external KolariVision Infrared Blue/NIR NDVI filter.

**Linear Averaging**  
((R + G + B)) / 3

**CVI: Version 1**  
((R + B) - (G) / (R + B) + (G)) / 3

**CVI: Version 2**  
((R + G) - (B) / (R + G) + (B)) / 3

**CVI: Version 3**  
1/((((R + B) - (G)) / ((R + B) + (G))) / 3)

**CVI: Version 4**  
((((R + G)/2) - B))/((((R + G)/2) + B))

**CVI: Version 5**  
1/((((R + B) - (G)) / ((R + B) + (G))))

**CVI: Version 6**  
((R + G) - (2 * B)) / ((R + B) + (2 * B))

**CVI: Version 7**  
((R + B) - (G) / ((R + B) + (G))) / 3

**CVI: Version 8**  
((((R + B)/2) - G))/((((R + B)/2) + G))

**CVI: Version 9**  
((((R + B) - (G)) / ((R + B) + (G))) / 3)
