[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/KhaderSheriff/polyp-3d-reconstruction/blob/main/demo/Demo.ipynb)

# Polyp 3D Surface Reconstruction from Monocular Endoscopy

This repository presents an end-to-end pipeline for estimating the three-dimensional morphology of colorectal polyps from a single monocular endoscopic image.

The proposed system integrates deep learning–based segmentation and depth estimation with geometric reconstruction techniques to recover polyp surface structure and morphology.

---

## Pipeline Overview

The processing pipeline consists of the following stages:

1. Polyp segmentation using a pretrained U-Net model  
2. Monocular depth estimation using MiDaS  
3. Depth–segmentation fusion to isolate the polyp region  
4. 3D point cloud generation and surface reconstruction  
5. Morphological measurement and visualization  

All models are used in inference mode only. No training is performed in this repository.

---

## Running the Demo

The complete pipeline is demonstrated in a single Jupyter notebook.

1. Open `demo/Demo.ipynb` in Google Colab  
2. Run all cells sequentially  
3. Provide an input endoscopic image and an optional ground-truth segmentation mask  

The notebook visualizes intermediate and final outputs, including segmentation results, depth maps, and 3D reconstructions.

---

## Data Availability

Due to dataset licensing restrictions, training datasets are not included in this repository.

A sample endoscopic image is provided for demonstration purposes.  
Pretrained models are automatically downloaded when running the notebook.

---

## Output

The demo generates the following outputs:

- Segmentation overlays  
- Relative depth maps  
- 3D point clouds and surface meshes  
- Quantitative morphological measurements (saved as CSV files)  

All depth-related measurements are reported in relative units.

---

## Notes and Limitations

- Pretrained models may not generalize perfectly to all endoscopic domains  
- MiDaS provides relative depth rather than absolute metric depth  
- Morphological measurements are approximate and intended for research demonstration  

---

## Usage in Research

This code is intended for research and educational purposes only.  
It is designed to demonstrate the feasibility of monocular 3D polyp morphology estimation and does not constitute a clinical diagnostic tool.

---

## Citation

Citation information will be added after conference publication.

