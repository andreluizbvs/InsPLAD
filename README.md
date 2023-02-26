# Inspection of Power Line Assets: the Dataset (InsPLAD) 

This repository stores InsPLAD, a dataset presented in the paper "InsPLAD: A Dataset and Benchmark for Power Line Asset Inspection in UAV Images".

You can download the dataset [here](https://drive.google.com/drive/folders/1psHiRyl7501YolnCcB8k55rTuAUcR9Ak?usp=sharing). Labels, when applicable, are in the zip files.

In the link above you will find three zip files:

- [InsPLAD-det.zip](https://drive.google.com/file/d/1Mu50QxKQ4NeLEhjEsTenLU97FxSd_HKD/view?usp=share_link) is an Object Detection dataset for Asset detection
- InsPLAD-fault folder:
  - [supervised_fault_classification.zip](https://drive.google.com/file/d/1Te3jRRM9gJXO8PwOoOoCPGY69Pq6YHUb/view?usp=share_link) is an Image Classification dataset for Fault Classification of the Assets
  - [unsupervised_anomaly_detection.zip](https://drive.google.com/file/d/1b_-gtyjMeO-Ndu_OaPrrSgSTwa31TWVz/view?usp=share_link) is an Unsupervised Anomaly Detection dataset also for Fault Classification of the Assets
  
## InsPLAD-det

- Object Detection dataset
- 17 classes (assets categories)
- 10,607 images

The image below shows at least one sample from each class in InsPLAD-det:

The table below summarizes other InsPLAD-det properties:

The table below benchmarks object detectors with InsPLAD-det:

## InsPLAD-fault

The image below shows samples from InsPLAD-fault:

The table below summarizes other InsPLAD-det properties:

### Supervised Fault Classification
- Image Classification dataset
- Five assets, two to three classes each (defect types, e.g., corrosion)
- X images

The table below benchmarks image classifiers with InsPLAD-fault:

### Unsupervised Anomaly Detection
- Anomaly Detection dataset
- Five assets, two classes each (normal or anomalous)  
- X images

The table below benchmarks anomaly detectors with InsPLAD-fault:
