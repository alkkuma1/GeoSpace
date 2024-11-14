# Indiana Pines Hyperspectral Data Visualization and Analysis

This repository contains an in-depth analysis and visualization of the Indiana Pines Hyperspectral (HS) dataset, conducted as part of a Data Visualization assignment for CS503. The dataset, captured by the Airborne Visible/Infrared Imaging Spectrometer (AVIRIS), provides spectral information across 220 bands, which are essential for applications in agriculture, environmental monitoring, and land cover classification.


## Dataset Overview

The Indiana Pines HS dataset consists of a 145x145 pixel image with each pixel containing spectral data across 220 bands, spanning the following ranges:

-   **Visible (VIS)**: 0.4 - 0.7 µm
-   **Near-Infrared (NIR)**: 0.7 - 1.3 µm
-   **Short-Wave Infrared (SWIR)**: 1.3 - 2.5 µm

The data is provided in `.mat` format, which is commonly used in MATLAB and compatible with Python for scientific data exchange.

## Project Objectives

This project involves various data analysis and visualization tasks aimed at gaining insights from the hyperspectral data. The key objectives are:

1.  Load and visualize the hyperspectral data cube.
2.  Generate and display a false color image using randomly selected spectral bands.
3.  Load and visualize the ground-truth image that annotates different classes in the dataset.
4.  Visualize the class distribution in a bar plot.
5.  Overlay ground-truth classes as a mask on the HS image for visual reference.
6.  Extract 1% of samples from each class, compute their mean spectral signatures, and plot them.
7.  Apply dimensionality reduction techniques (PCA and t-SNE) and display scatter plots for the first two components of each method.
8.  Reconstruct and display the image using the first principal component of PCA and the first component of t-SNE.

## Repository Structure

-   `notebooks/` - Contains the Jupyter notebook with the analysis and visualizations.
-   `data/` - Stores the `.mat` hyperspectral dataset and ground-truth files (ensure they are placed here before running the notebook).
-   `images/` - Generated visualizations, including plots and reconstructed images.
-   `README.md` - This file.

## Prerequisites

```pip install scikit-learn matplotlib spectral tqdm```


## Getting Started

1. Clone the repository:
``` git clone https://https://github.com/alkkuma1/GeoSpace.git```
``` cd GeoSpace ```
2. Download the `.mat` file containing the Indiana Pines dataset.
3.  Open and run the notebook to execute the analysis.

## Results

-   **False Color Image**: A composite image using three randomly selected spectral bands.
-   **Class Distribution**: Bar plot showing the number of samples per class.
-   **Mean Spectral Signatures**: Spectral signature plots for sampled classes.
-   **Dimensionality Reduction Plots**: Scatter plots for PCA and t-SNE, visualizing clusters within classes.
-   **Image Reconstruction**: Reconstructed images using the primary component from PCA and t-SNE.


# References


  

- [1] S.Enayat Hosseini aria et al. http://dx.doi.org/10.1117/1.JRS.11.046010
- [2] Refka Hanachi et al. DOIhttps://doi.org/10.1007/s00521-023-09275-5
-   [3] Md. Moazzem Hossain doi.org/10.3390/electronics12092082
-   [4] Behnood Rasti DOI: 10.13140/RG.2.1.4097.4247
-   [5] https://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes
