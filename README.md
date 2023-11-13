# Inspection of Power Line Assets: the Dataset (InsPLAD) 

This repository stores InsPLAD, a dataset introduced in "_InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images_" [arXiv](https://arxiv.org/abs/2311.01619). InsPLAD is also used in "_Attention Modules Improve Image-Level Anomaly Detection for Industrial Inspection: A DifferNet Case Study_" [arXiv](https://arxiv.org/abs/2311.02747).

You can download the dataset [**here**](https://drive.google.com/drive/folders/1psHiRyl7501YolnCcB8k55rTuAUcR9Ak?usp=drive_link) (Google Drive). Labels, when applicable, are in the zip files.

**Three datasets in one**. In the link above, you will find three zip files:

- ```InsPLAD-det.zip``` is an **Object Detection** dataset for Asset detection
- InsPLAD-fault folder:
  - ```supervised_fault_classification.zip``` is an **Image Classification** dataset for Fault Classification of the Assets
  - ```unsupervised_anomaly_detection.zip``` is an **Unsupervised Anomaly Detection** dataset also for Fault Classification of the Assets

Here is a straightforward workflow that can be applied when using InsPLAD:

<img src="https://i.imgur.com/P2awEoO.png" width="650">

The black boxes indicate the function of each sub-dataset in the Power line domain and which Computer Vision task (in parentheses) should be used for each sub-dataset.

## Citing
If you use InsPLAD in your research, please cite it:
```
@article{doi:10.1080/01431161.2023.2283900,
author  = {Vieira e Silva,André Luiz and Felix,Heitor and Simões,Francisco Paulo and Teichrieb,Veronica and dos Santos,Michel and Santiago,Hemir and Sgotti,Virgínia and Lott Neto,Henrique},
title   = {InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images},
journal = {International Journal of Remote Sensing},
year    = {2023},
doi     = {10.1080/01431161.2023.2283900},
}

@InProceedings{Vieira_2024_WACV,
    author    = {{Vieira e Silva}, André Luiz Buarque and Simões, Francisco and Kowerko, Danny and Schlosser, Tobias and Battisti, Felipe and Teichrieb, Veronica},
    title     = {Attention Modules Improve Image-Level Anomaly Detection for Industrial Inspection: A DifferNet Case Study},
    booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
    month     = {January},
    year      = {2024},
    pages     = {(to appear)}
}
```

## 1. InsPLAD-det

### Properties
- Object Detection dataset
- 17 classes (assets categories)
- 10,607 total images
- 28,933 total instances
- Other properties:

<img src="https://i.imgur.com/PEAjChU.png" width="650">


### Samples

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

<img src="https://i.imgur.com/miLnAKH.png" width="850">


