# 3D Tree Crown Analysis from LiDAR Data

This repository contains a pipeline for analyzing tree crown metrics and generating 3D visualizations from LiDAR data, demonstrated on [AHN4](https://www.ahn.nl/) Dutch elevation data. The workflow includes point cloud processing, classification, and geometric analysis of tree structures.

The pipeline consists of six main steps (see [`3d_tree_crown.ipynb`](./3d_tree_crown.ipynb)):

1. **Data Loading**: Read and process LAS point cloud files
2. **Classification**: Separate ground and vegetation points using AHN4 classification labels
3. **Filtering**: Remove outliers using Z-score statistical analysis
4. **DEM Generation**: Create Digital Elevation Models using Kriging interpolation
5. **3D Visualization**: Interactive point cloud visualization with Open3D
6. **Metric Extraction**: Calculate tree height, diameter, and crown volume

<b>Example Visualizations:</b>

| ![Raw Point Cloud](./assets/screenshots/raw_points.png) | ![Classified Points](./assets/screenshots/classified.png) |
|:---:|:---:|
| Raw LiDAR Point Cloud | Classified Ground & Vegetation |

| ![DEM Visualization](./assets/screenshots/dem.png) | ![3D Crown Analysis](./assets/screenshots/3d_analysis.png) |
|:---:|:---:|
| Digital Elevation Model | 3D Crown Metrics Visualization |

## Folder Structure
