# InsPLAD: Inspection of Power Line Assets Dataset

This repository stores InsPLAD, a dataset introduced in "_InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images_" [IJRS](https://www.tandfonline.com/doi/full/10.1080/01431161.2023.2283900) | [arXiv](https://arxiv.org/abs/2311.01619). InsPLAD is also used in "_Attention Modules Improve Image-Level Anomaly Detection for Industrial Inspection: A DifferNet Case Study_" [arXiv](https://arxiv.org/abs/2311.02747).

## Abstract

Power line maintenance and inspection are essential to avoid power supply interruptions, reducing its high social and financial impacts yearly. Automating power line visual inspections remains a relevant open problem for the industry due to the lack of public real-world datasets of power line components and their various defects to foster new research. This paper introduces InsPLAD, a Power Line Asset Inspection Dataset and Benchmark containing 10,607 high-resolution Unmanned Aerial Vehicles colour images. The dataset contains seventeen unique power line assets captured from real-world operating power lines. Additionally, five of those assets present six defects: four of which are corrosion, one is a broken component, and one is a bird's nest presence. All assets were labelled according to their condition, whether normal or the defect name found on an image level. We thoroughly evaluate state-of-the-art and popular methods for three image-level computer vision tasks covered by InsPLAD: object detection, through the AP metric; defect classification, through Balanced Accuracy; and anomaly detection, through the AUROC metric. InsPLAD offers various vision challenges from uncontrolled environments, such as multi-scale objects, multi-size class instances, multiple objects per image, intra-class variation, cluttered background, distinct point-of-views, perspective distortion, occlusion, and varied lighting conditions. To the best of our knowledge, InsPLAD is the first large real-world dataset and benchmark for power line asset inspection with multiple components and defects for various computer vision tasks, with a potential impact to improve state-of-the-art methods in the field. It will be publicly available in its integrity on a repository with a thorough description.

You can download the dataset [**here**](https://drive.google.com/drive/folders/1psHiRyl7501YolnCcB8k55rTuAUcR9Ak?usp=drive_link) (Google Drive). Labels, when applicable, are in the zip files.

**Three datasets in one**. In the link above, you will find three zip files:

- ```InsPLAD-det.zip``` is an **Object Detection** dataset for Asset detection
- InsPLAD-fault folder:
  - ```supervised_fault_classification.zip``` is an **Image Classification** dataset for Fault Classification of the Assets
  - ```unsupervised_anomaly_detection.zip``` is an **Unsupervised Anomaly Detection** dataset also for Fault Classification of the Assets

Here is a straightforward workflow that can be applied when using InsPLAD:

<img src="https://i.imgur.com/P2awEoO.png" width="650">

The black boxes indicate the function of each sub-dataset in the Power line domain and which Computer Vision task (in parentheses) should be used for each sub-dataset.

## 1. InsPLAD-det

### Properties
- Object Detection dataset
- 17 classes (assets categories)
- 10,607 total images
- 28,933 total instances
- Other properties:

<img src="https://i.imgur.com/PEAjChU.png" width="650">


### Samples
Different bounding box colors mean different classes (not normal/defective objects)

<img src="https://i.imgur.com/s0ofrRH.png" width="850">

<!--
#### Benchmark

<img src="https://i.imgur.com/UxyGAqg.png" width="600"> 
-->

## 2. InsPLAD-fault

InsPLAD-fault is generated from InsPLAD-det. The annotated objects are cropped and classified into normal/defective. 

### Properties

<img src="https://i.imgur.com/fz5sAsI.png" width="650">

### 2.1 Supervised Fault Classification
- Image Classification dataset
- Five assets, 2 to 3 classes each (defect types, e.g., corrosion)
- Other properties in the table above

<!--
#### Benchmark

<img src="https://i.imgur.com/HkRHjJD.png" width="600">
-->

### 2.2 Unsupervised Anomaly Detection
- Anomaly Detection dataset
- Five assets, 2 classes each (normal or anomalous)
- Other properties in the table above



<!--
#### Benchmark

<img src="https://i.imgur.com/GaKzagk.png" width="600">
-->

### Samples
Normal on top in green and defective at the bottom in red

<img src="https://i.imgur.com/Ocq2kl7.png" width="1000">

## Citing
If you use InsPLAD in your research, please cite it:
```
@article{doi:10.1080/01431161.2023.2283900,
   author    = {André Luiz Buarque Vieira e Silva, Heitor de Castro Felix, Franscisco Paulo Magalhães Simões, Veronica Teichrieb, Michel dos Santos, Hemir Santiago, Virginia Sgotti and Henrique Lott Neto},
   title     = {InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images},
   journal   = {International Journal of Remote Sensing},
   volume    = {0},
   number    = {0},
   pages     = {1-27},
   year      = {2023},
   publisher = {Taylor & Francis},
   doi       = {10.1080/01431161.2023.2283900},
   URL       = {https://doi.org/10.1080/01431161.2023.2283900},
   eprint    = {https://doi.org/10.1080/01431161.2023.2283900},
}

@InProceedings{Vieira_2024_WACV,
    author    = {Vieira e Silva, André Luiz Buarque and Simões, Francisco and Kowerko, Danny and Schlosser, Tobias and Battisti, Felipe and Teichrieb, Veronica},
    title     = {Attention Modules Improve Image-Level Anomaly Detection for Industrial Inspection: A DifferNet Case Study},
    booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
    month     = {January},
    year      = {2024},
    pages     = {(to appear)}
}
```
