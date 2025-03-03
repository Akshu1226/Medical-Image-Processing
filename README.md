# MEDICAL IMAGE PROCESSING
## Introduction:
Brain tumors are abnormal masses of cells that are found within the brain and can be benign or malignant. Proper detection and accurate segmentation of brain tumors are both crucial in enabling appropriate diagnosis, treatment planning, and improved patient survival.
Magnetic Resonance Imaging (MRI) is the imaging modality of choice for the detection of brain tumors because it can capture the fine details of soft tissues. Manual segmentation of MRI scans is time-consuming, error-prone, and high in expertise. Automatic segmentation using deep learning offers a quicker, more precise, and reproducible method of marking tumor areas.

## Dataset:
The data set used in this project is the Brain Tumor MRI Dataset, downloaded from Kaggle. The data set comprises MRI scan images labeled to indicate either the presence or absence of brain tumors. MRI or Magnetic Resonance Imaging is a frequently used imaging modality in medical imaging due to the fact that it is able to represent detailed visualization of soft tissues without exposure to radiation.

–Dataset Composition
The data contains:

1.MRI scans of the brain tumor in various stages.

2.Tagged tumor masks showing the tumor area. 

3.Various types of tumours, making classification-based segmentation possible.

Dataset:-https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

## Deep Learning Models Used:
U-Net – A fully convolutional encoder-decoder network with skip connections that helps preserve fine tumor details, making it highly effective for medical image segmentation.

PSPNet – Uses a pyramid pooling module to capture multi-scale tumor structures, improving segmentation accuracy for both small and large tumors.

VGG-19 – A deep convolutional neural network (CNN) with 19 layers, known for its strong feature extraction capabilities and effectiveness in tumor classification.

## Performance Evaluation:
1️.Dice Coefficient – Measures the overlap between predicted and actual tumor regions, with higher values indicating better segmentation accuracy.

2️.Intersection over Union (IoU) – Calculates the ratio of correctly predicted tumor pixels to the total tumor pixels in both ground truth and prediction.

3️.Accuracy – Represents the percentage of correctly classified pixels in the MRI scans, showing the overall segmentation performance.

4️.Precision – Indicates how many of the predicted tumor pixels are actually tumors, reducing false positives.

5️.Recall – Measures how many actual tumor pixels were correctly identified, reducing false negatives.

## Training Process:
1️⃣ Dataset Splitting – The dataset is divided into training and testing sets to ensure proper model evaluation.

2️⃣ Preprocessing – Techniques like normalization, data augmentation, noise reduction, and contrast enhancement are applied to improve model performance.

3️⃣ Hyperparameter Tuning – Parameters such as learning rate, batch size, and dropout rate are optimized for better training efficiency.

4️⃣ Model Training – The deep learning models are trained using MRI images with labeled tumor regions to learn accurate segmentation patterns.

5️⃣ Loss Function Optimization – A loss function like Dice Loss or Cross-Entropy Loss is used to minimize segmentation errors.

6️⃣ Validation and Testing – The trained models are tested on unseen MRI scans, and their performance is evaluated using Dice Coefficient, IoU, Precision, and Recall.

## Results and Visualizations:

 Segmentation Output – The models generate segmented tumor regions on MRI scans, highlighting the affected areas.

 Performance Comparison – U-Net achieves the highest accuracy, while PSPNet captures multi-scale tumor regions, and VGG-19 provides strong feature extraction.

 Dice Coefficient & IoU Scores – Higher Dice and IoU values indicate better segmentation accuracy, with U-Net performing the best.

 Graphical Analysis – Loss curves, accuracy plots, and confusion matrices visualize model performance across training and testing phases.

 Overlay Visualization – Predicted tumor masks are overlaid on the original MRI scans to visually assess segmentation quality.
 ![image](https://github.com/user-attachments/assets/eb5518de-edde-4f8c-b860-46fafee03042)



