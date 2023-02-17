# Liver-Vessel-Segment and other Organ Vessel Segment


#### <a href="#id_1">Part One: Liver Vessel Segmentation Review </a>
Date  |  Journal  |  Title |
:---- |----------:|--------:
2018  |  XXX   | Computational Methods for Liver Vessel Segmentation in Medical Imaging A Review |
2018  |  XXX   | Techniques and Algorithms for Hepatic Vessel Skeletonization in Medical Images: A Survey


&nbsp; 
&nbsp;  
#### <a href="#id_1">Part Two: Based on Traditional models</a>
Date  |  Data  | Module | Title|
:---- |-------:|-------:|------:
2018  |  XXX   |  XXX   | Accurate liver vessel segmentation via active contour model with dense vessel candidates |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |



&nbsp; 
&nbsp;  
#### <a href="#id_1">Part Three: Based on FCN models</a>
Date  |  Data  | Module | Title|
:---- |-------:|-------:|------:
2022  |  XXX   |  XXX   | HPM-Net: Hierarchical progressive multiscale network for liver vessel segmentation in CT images |
2018  |  XXX   |  XXX   | Automatic 3-d skeleton-based segmentation of liver vessels from mri and ct for couinaud representation |
2019  |  XXX   |  XXX   | Automatic segmentation methods for liver and hepatic vessels from CT and MRI volumes, applied to the Couinaud scheme |
2019  |  XXX   |  XXX   | VesselNet A deep convolutional neural network with multi pathways for robust hepatic vessel segmentation |
2020  |  XXX   |  XXX   | Attention-guided deep neural network with multi-scale feature fusion for liver vessel segmentation |
2020  |  XXX   |  XXX   | Channel width optimized neural networks for liver and vessel segmentation in liver iron quantification |
2020  |  XXX   |  XXX   | Training liver vessel segmentation deep neural networks on noisy labels from contrast CT imaging |
2021  |  XXX   |  XXX   | Effects of enhancement on deep learning based hepatic vessel segmentation |
2021  |  XXX   |  XXX   | Exploiting full Resolution Feature Context for Liver Tumor and Vessel Segmentation via Fusion Encoder Application to Liver Tumor and Vessel 3D reconstruction |
2022  |  XXX   |  XXX   | Hierarchical deep network with uncertainty-aware semi-supervised learning for vessel segmentation |
2022  |  XXX   |  XXX   | Robust Deep 3D Blood Vessel Segmentation Using Structural Priors |
2022  |  XXX   |  XXX   | Structural Prior Models for 3-D Deep Vessel Segmentation |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |



&nbsp; 
&nbsp;  
#### <a href="#id_1">Part Four: Based on V-Net models</a>
Date  |  Data  | Module | Title|
:---- |-------:|-------:|------:
2021  |  XXX   |  XXX   | Liver vessel segmentation based on inter-scale V-Net |
2021  |  XXX   |  XXX   | DV-Net Accurate liver vessel segmentation via dense connection model with D-BCE loss function |
2020  |  XXX   |  XXX   | Liver vessel segmentation based on densely connected three-dimensional fully convolutional neural network |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |



&nbsp; 
&nbsp;  
#### <a href="#id_1">Part Four: Based on U-Net models</a>
Date  |  Data  | Module | Title|
:---- |-------:|-------:|------:
2019  |  XXX   |  XXX   | Liver vessels segmentation based on 3d residual U-NET |
20XX  |  XXX   |  XXX   | SU-UNet: A Novel Self-Updating Network for Hepatic Vessel Segmentation in CT Images |
2018  |  XXX   |  XXX   | Robust liver vessel extraction using 3D U-Net with variant dice loss function |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |



&nbsp; 
&nbsp;  
#### <a href="#id_1">Part Five: Based on Transformer models</a>
Date  |  Data  | Module | Title|
:---- |-------:|-------:|------:
2021  |  XXX   |  XXX   | Hepatic Vessel segmentation based on 3D swin-transformer with inductive biased multi-head self-attention |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |
20XX  |  XXX   |  XXX   | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA |



&nbsp; 
&nbsp;  
#### <a href="#id_1">Part Six: Other Organ Vessel Segment</a>
Date  |  Organ  | Module | Joural | Title|
:---- |-------:|-------:|-------:|------:
2022  | head-neck | dual-task | Computer Methods and Programs in Biomedicine | Simultaneous vessel segmentation and unenhanced prediction using self-supervised dual-task learning in 3D CTA (SVSUP) |



# Liver Vessel Segment Data Preprocessing
[1] Robust liver vessel extraction using 3D U-Net with variant dice loss function(Computers in Biology and Medicine, 2018)    
Preprocessing consists of 3 steps: (1) CT values are limited to [0400]
HU to focus on the intensity range of the liver. (2) CT images and annotated
images are cropped to the liver area based on the pre-segmented
liver mask, and adjusted to the size of 288×288×96. For local
datasets, the liver mask is obtained by our previous liver segmentation
method [27]. (3) Images are normalized to zero mean and unit variance.
Since most liver vessels are quite small, we trained images with
their original resolution if it was in a reasonable range to prevent artifact
errors caused by resampling. For data with slice thickness smaller
than 0.8mm or larger than 2.5 mm, we used a coordinate transform and
cubic spline interpolation to transfer the data into a slice thickness of
1.6 mm.

[2] LIVER VESSELS SEGMENTATION BASED ON 3D RESIDUAL U-NET (2019)  
To improve the segmentation performance and effectively
prevent overfitting during training, we have applied many image
amplification methods to increase our training set, which
contains elastic deformation and a combined transformation,
where the combined transformation includes translation, rotation
and gray value transformation. In our experiment, the
rotation angle is randomly selected from -20 to +20, the
translation is between -52 and +52 pixels, and gray value
transformation is achieved by multiply the gray value with
a random number ranging from 0.8 to 1.

[3]Attention-Guided Deep Neural Network With Multi-Scale Feature Fusion for Liver Vessel Segmentation (IEEE Journal of and Health Informatics, 2021)  
CT images and annotated images are cropped to the liver area based on the pre-segmented liver mask, then werandomly crop patches of size
256 × 256 × 64 from the liver area for training. To eliminate the overfitting problem, we also adopt data augmentation to enrich the training data. All computations were performed using 8 NVIDIA Titan RTX GPUs with 24 GB memory. The initial learning rate is set to 10−4 and divided by 10 every 5000 epoch.
(1)The range of pixel spacing is 0.55 to 0.80 mm.

[4] Liver vessel segmentation based on densely connected three-dimensional fully convolutional neural network
To focus on the liver intensity range, the CT value range is limited to [0,400] HU. Assuming that there are n voxels in the liver area, x is the pixel value of the i-th point in the liver area, and the formula is as follows:

[5]TRAINING LIVER VESSEL SEGMENTATION DEEP NEURAL NETWORKS ON NOISY LABELS FROM CONTRAST CT IMAGING (ISBI, 2020)
Then we truncate the intensity of all volumes to the range of [-100, 250] HU to remove the irrelevant details and normalized them by subtracting the mean.

[6] HPM-Net: Hierarchical progressive multiscale network for liver vessel segmentation in CT images (Computer Methods and Programs in Biomedicine, 2022)  
The purpose of data preprocessing is to improve the contrast of vascular pixels and facilitate network feature extraction. The pre- treatment steps are as follows:
(1)
The CT value of images is limited to [-10 0,30 0] HU, which filters out other organs to better focus on the liver regions;
(2)
To avoid the influence of the tissue around the liver and reduce the amount of computation, the CT images and annotated im- ages were cropped to the liver region based on the liver mask obtained by the liver segmentation method, and the size was adjusted to 288 ×288 ×96. There are some data with Z-axis less than 96, and we intercepted the size of 96 on the original data with the liver as the center.
(3)
All images are standardized by removing the mean and divid- ing them by the standard deviation, and finally standardized to make all data mapped to the range of [0,1];
(4)
Random scaling, rotation, and mirroring operations are used to expand data. In our experiment, the scaling operation first randomly crops to 192 ∗192 ∗96 size, and then scales down to 96 ∗96 ∗96 size using the nearest neighbor interpolation method. Rotation operation is randomly rotated to 90 ◦, 180 ◦and 270 ◦. The mirroring transformation is mainly horizontal, vertical and diagonal mirroring.
