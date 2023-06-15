# Brain-Tumor-Segmentation
Brain tumor segmentation is a crucial task in medical imaging that involves identifying and delineating the boundaries of tumors present in brain images. It plays a significant role in diagnosis, treatment planning, and monitoring the progress of brain cancer patients. Segmentation enables clinicians to accurately measure tumor size, assess its growth or regression, and evaluate treatment response.

There are various techniques and algorithms employed for brain tumor segmentation, ranging from traditional methods to more advanced deep learning approaches. Here are a few commonly used techniques:

Manual Segmentation: This approach involves manual delineation of tumor boundaries by an expert radiologist or physician. It is time-consuming and subject to inter-observer variability, but it can provide accurate results when performed by experienced professionals.

Thresholding: Thresholding techniques involve setting a threshold value to separate tumor regions from the background based on pixel intensity. It is a simple method but may not be suitable for complex tumors with irregular shapes or overlapping intensities.

Region Growing: Region growing algorithms start from a seed point and iteratively expand the region by adding neighboring pixels that meet specific criteria, such as intensity similarity. It can handle tumors with irregular shapes but may be sensitive to seed point selection.

Active Contour Models: Active contour, or snakes


# Problem definiton
**Segmentation of gliomas in pre-operative MRI scans.**

*Each pixel on image must be labeled:*
* Pixel is part of a tumor area (1 or 2 or 3) -> can be one of multiple classes / sub-regions
* Anything else -> pixel is not on a tumor region (0)

The sub-regions of tumor considered for evaluation are: 1) the "enhancing tumor" (ET), 2) the "tumor core" (TC), and 3) the "whole tumor" (WT)
The provided segmentation labels have values of 1 for NCR & NET, 2 for ED, 4 for ET, and 0 for everything else.
