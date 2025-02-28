# MEDICAL IMAGE PROCESSING
## Introduction:
Brain tumors are abnormal masses of cells that are found within the brain and can be benign or malignant. Proper detection and accurate segmentation of brain tumors are both crucial in enabling appropriate diagnosis, treatment planning, and improved patient survival.
Magnetic Resonance Imaging (MRI) is the imaging modality of choice for the detection of brain tumors because it can capture the fine details of soft tissues. Manual segmentation of MRI scans is time-consuming, error-prone, and high in expertise. Automatic segmentation using deep learning offers a quicker, more precise, and reproducible method of marking tumor areas.
## Dataset:
The data set used in this project is the Brain Tumor MRI Dataset, downloaded from Kaggle. The data set comprises MRI scan images labeled to indicate either the presence or absence of brain tumors. MRI or Magnetic Resonance Imaging is a frequently used imaging modality in medical imaging due to the fact that it is able to represent detailed visualization of soft tissues without exposure to radiation.

2️⃣ Dataset Composition
The data contains:

1.MRI scans of the brain tumor in various stages.

2.Tagged tumor masks showing the tumor area. 

3.Various types of tumours, making classification-based segmentation possible.

Dataset:-https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

## Deep Learning Models Used
U-Net – A fully convolutional encoder-decoder network with skip connections that helps preserve fine tumor details, making it highly effective for medical image segmentation.

PSPNet – Uses a pyramid pooling module to capture multi-scale tumor structures, improving segmentation accuracy for both small and large tumors.

VGG-19 – A deep convolutional neural network (CNN) with 19 layers, known for its strong feature extraction capabilities and effectiveness in tumor classification.

## Performance Evaluation
1️.Dice Coefficient – Measures the overlap between predicted and actual tumor regions, with higher values indicating better segmentation accuracy.

2️.Intersection over Union (IoU) – Calculates the ratio of correctly predicted tumor pixels to the total tumor pixels in both ground truth and prediction.

3️.Accuracy – Represents the percentage of correctly classified pixels in the MRI scans, showing the overall segmentation performance.

4️.Precision – Indicates how many of the predicted tumor pixels are actually tumors, reducing false positives.

5️.Recall – Measures how many actual tumor pixels were correctly identified, reducing false negatives.



