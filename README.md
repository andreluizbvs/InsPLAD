# Inspection of Power Line Assets: the Dataset (InsPLAD) 

This repository stores InsPLAD, a dataset presented in "**InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images**" ([arXiv]()).

You can download the dataset [**here**](https://drive.google.com/drive/folders/1psHiRyl7501YolnCcB8k55rTuAUcR9Ak?usp=sharing) (Google Drive). Labels, when applicable, are in the zip files.

**THREE datasets in one**. In the link above you will find three zip files:

- ```InsPLAD-det.zip``` is an **Object Detection dataset** for Asset detection
- InsPLAD-fault folder:
  - ```supervised_fault_classification.zip``` is an **Image Classification dataset** for Fault Classification of the Assets
  - ```unsupervised_anomaly_detection.zip``` is an **Unsupervised Anomaly Detection dataset** also for Fault Classification of the Assets

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



## Citing

```
@misc{vieiraesilva2023insplad,
      title={InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images}, 
      author={André Luiz Buarque Vieira-e-Silva and Heitor de Castro Felix and Francisco Paulo Magalhães Simões and Veronica Teichrieb and Michel dos Santos and Hemir Santiago and Virginia Sgotti and Henrique Lott-Neto},
      year={2023},
      eprint={-},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
