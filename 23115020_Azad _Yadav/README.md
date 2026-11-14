# Reproducible Segmentation Experiment: Retinal Vessel Extraction

This repository contains the code and report for Unit 3 Assignment B. The experiment investigates the impact of atrous (dilated) convolution on spatial context and class imbalance in medical image segmentation.

## Reproducibility Requirements
* **Dataset:** [DRIVE (Digital Retinal Images for Vessel Extraction)](https://www.kaggle.com/datasets/andrewmvd/drive-digital-retinal-images-for-vessel-extraction)
* **Environment:** Kaggle Notebook (GPU T4 x2)
* **Python Dependencies:** `torch`, `numpy`, `pillow`, `matplotlib`
* **Seed:** `42` (Fixed across PyTorch, CUDA, and NumPy)

## Execution
The experiment is fully contained within `segmentation_experiment.ipynb`. To reproduce:
1. Load the notebook into Kaggle and attach the DRIVE dataset.
2. Run all cells. The script will automatically parse the data, train both the Baseline U-Net and the Dilated Bottleneck U-Net for 30 epochs, and output the latency, parameter counts, and mIoU metrics.