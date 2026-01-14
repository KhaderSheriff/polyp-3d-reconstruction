# Polyp 3D Surface Reconstruction from Monocular Endoscopy

This repository demonstrates an end-to-end pipeline for estimating the 3D morphology of polyps from a single monocular endoscopic image.

## Pipeline
- Polyp segmentation using pretrained U-Net
- Monocular depth estimation using MiDaS
- Depth–segmentation fusion
- 3D reconstruction and surface visualization
- Morphological measurements

## Running the Demo
Open `demo/Demo.ipynb` in Google Colab and run all cells sequentially.

## Data
Due to dataset licensing restrictions, training datasets are not included.
A sample image is provided for demonstration purposes.

## Notes
- Models are used for inference only.
- Depth values are relative, not absolute.
