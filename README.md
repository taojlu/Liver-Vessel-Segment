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
[1] Robust liver vessel extraction using 3D U-Net with variant dice loss function  
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
