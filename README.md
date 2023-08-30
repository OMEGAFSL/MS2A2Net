# MS2A2Net
## Multi-Scale Self-Attention Aggregation Network for Few-Shot Aerial Imagery Segmentation
This repository contains the official implementation of Multi-Scale Self-Attention Aggregation Network for Few-Shot Aerial Imagery Segmentation(MS2A2Net).

## Requirements
This repo requires the following:  
`numpy==1.19.2`  
`pandas==1.3.5`  
`Pillow==9.2.0`  
`scipy==1.6.2`  
`torch==1.8.2`  
`torchvision==0.9.2`  
`opencv==4.6.0.66`  
`tensorboard 1.14`  


## Datasets
Furthermore, to enrich the available datasets of few-shot remote sensing aerial imagery, we reconstructed two novel
datasets, called DLRSD-4i and iSAID-4i, according to the paradigm of few-shot segmentation.  
### DLRSD-4i
We reconstructed a novel few-shot remote sensing aerial image segmentation dataset, dubbed DLRSD-4i , from the DLRSD dataset, according to the paradigm of few-shot segmentation. In DLRSD dataset, there are 17 segmentation targets in total, but considering that the cases in the category ”filed” are basically all foreground information without reference value
for the background information, so it is discarded in DLRSD-4i, leaving only the following 16 segmentation targets. This
dataset has a total of 7,002 images with 256 × 256 pixels. These 16 segmented object classes in the DLRSD-4i dataset
are equally divided into 4 folds, 3 of which are used for training and 1 for testing. The DLRSD-4i dataset is small in
scale and the scene differences are large, which puts forward strict requirements on the fast generalization ability of the few-shot segmentation algorithms.  
### iSAID-4i
Yao et al. reintegrated the iSAID dataset according to the commonly used few-shot semantic segmentation paradigm and released the iSAID-5i dataset.
To enrich the diversity of few-shot remote sensing image segmentation datasets, especially taking 4 categories as a split option, based on the iSAID-5i dataset, we added the
category of buildings from the Massachusetts dataset , and reconstructed a novel few-shot remote sensing segmentation
dataset named iSAID-4i. The specific information of each split in the iSAID-4i dataset is shown in Table II. The iSAID-4i dataset has 28,214 images with a size of 256×256 pixels. Specifically, the iSAID-4i dataset has a total of 16 categories of segmentation targets, and the cross-validation strategy is implemented, i.e., 4 categories are used for testing
and the other 12 categories are used for training. The large size and rich scenes of the iSAID-4i dataset impose stringent
requirements on few-shot segmentation algorithms to deal with high inter-class similarity and large intra-class variability.  
### download
You can download iSAID at this [Baidu Netdisk](https://pan.baidu.com/s/1geZuig2p_HwJgerFGHRG9w) by the password *3035*, or download at this [Google Drive](https://drive.google.com/file/d/1GzTa9X6QzAjcySzKPx_wGri56jzeMf4-/view?usp=drive_link)  
You can also download DLRSD at this [Baidu Netdisk](https://pan.baidu.com/s/1oYovKl7eEAzgseTPGe16RQ) by the password *7002*, or download at this [Google Drive](https://drive.google.com/file/d/1JsRMb6870YE7nPoYcRttxjeKgM-dRXDm/view?usp=drive_link)  

## Comparison method
HSNet: <https://github.com/juhongm999/hsnet>  
VAT: <https://github.com/Seokju-Cho/Volumetric-Aggregation-Transformer>  
HDMNet: <https://github.com/Pbihao/HDMNet>  
BAM: <https://github.com/chunbolang/BAM>  
PFENet: <https://github.com/dvlab-research/PFENet>  

## Evaluation
### Comparison on the DLRSD-4i dataset
![DLRSD-4i](https://github.com/OMEGAFSL/MS2A2Net/assets/110706904/64ce3dca-541e-497d-9600-6f0659a1eb66)
### Comparison on the iSAID-4i dataset
![iSAID-4i](https://github.com/OMEGAFSL/MS2A2Net/assets/110706904/96f82a5d-0161-4dc4-ab50-9624ce4c7179)



