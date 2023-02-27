# Inspection of Power Line Assets: the Dataset (InsPLAD) 

This repository stores InsPLAD, a dataset presented in "**InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images**" ([arXiv]()).

You can download the dataset [**here**](https://drive.google.com/drive/folders/1psHiRyl7501YolnCcB8k55rTuAUcR9Ak?usp=sharing) (Google Drive). Labels, when applicable, are in the zip files.

In the link above you will find three zip files:

- ```InsPLAD-det.zip``` is an Object Detection dataset for Asset detection
- InsPLAD-fault folder:
  - ```supervised_fault_classification.zip``` is an Image Classification dataset for Fault Classification of the Assets
  - ```unsupervised_anomaly_detection.zip``` is an Unsupervised Anomaly Detection dataset also for Fault Classification of the Assets
  
## InsPLAD-det


### Properties
- Object Detection dataset
- 17 classes (assets categories)
- 10,607 total images
- 28,933 total instances
- Other properties:

<img src="https://i.imgur.com/PEAjChU.png" width="600">


### Samples

<img src="https://i.imgur.com/s0ofrRH.png" width="600">

<!--
#### Benchmark

<img src="https://i.imgur.com/UxyGAqg.png" width="600"> 
-->

## InsPLAD-fault

InsPLAD-fault is generated from InsPLAD-det. The annotated objects are cropped and classified into normal/defective. 

### Properties

<img src="https://i.imgur.com/fz5sAsI.png" width="600">

#### Supervised Fault Classification
- Image Classification dataset
- Five assets, 2 to 3 classes each (defect types, e.g., corrosion)
- Other properties in the table above

<!--
#### Benchmark

<img src="https://i.imgur.com/HkRHjJD.png" width="600">
-->

#### Unsupervised Anomaly Detection
- Anomaly Detection dataset
- Five assets, 2 classes each (normal or anomalous)
- Other properties in the table above



<!--
#### Benchmark

<img src="https://i.imgur.com/GaKzagk.png" width="600">
-->

### Samples

<img src="https://i.imgur.com/miLnAKH.png" width="600">



## Citing

```
@misc{vieiraesilva2021stn,
      title={STN PLAD: A Dataset for Multi-Size Power Line Assets Detection in High-Resolution UAV Images}, 
      author={André Luiz Buarque Vieira-e-Silva and Heitor de Castro Felix and Francisco Paulo Magalhães Simões and Veronica Teichrieb and Michel dos Santos and Hemir Santiago and Virginia Sgotti and Henrique Lott-Neto},
      year={2023},
      eprint={-},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
