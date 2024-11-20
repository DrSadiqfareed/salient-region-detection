# Salient Region Detection Using Sparse Reconstruction and Graph-Based Ranking

This project implements a **salient region detection algorithm** inspired by the paper _"Salient region detection through sparse reconstruction and graph-based ranking"_. The method combines **superpixel segmentation**, **sparse saliency**, **graph-based ranking**, and **Bayesian integration** to generate precise and smooth saliency maps.

---

## Features

1. **Superpixel Segmentation**:
   - Divides the image into meaningful, compact regions using the SLIC algorithm.
   
2. **Sparse Saliency**:
   - Computes saliency by measuring the contrast between superpixels and boundary regions.

3. **Graph-Based Ranking**:
   - Refines saliency scores using graph-based Laplacian ranking.

4. **Bayesian Integration**:
   - Combines sparse saliency and graph-based saliency into a unified, robust saliency map.

5. **Visualization**:
   - Generates a heatmap-style saliency map for intuitive visualization.

---

## Installation

### Prerequisites

Ensure you have Python 3.7+ installed along with the following libraries:
- `numpy`
- `opencv-python`
- `scikit-image`
- `scipy`
- `matplotlib`

Install the required dependencies using pip:

pip install numpy opencv-python scikit-image scipy matplotlib

Usage
Clone the repository:
git clone https://github.com/yourusername/salient-region-detection.git
cd salient-region-detection
Place your input image in the project directory. For example, save it as example_image.jpg.

Run the detection script:
python salient_region_detection.py

View the resulting saliency map:
The output will display the heatmap of the saliency map.

File Structure

├── salient_region_detection.py  # Main saliency detection script
├── example_image.jpg            # Example input image
├── README.md                    # Documentation

Example Output
Input Image


Saliency Map

Algorithm Workflow

Input Image: The image is processed for salient region detection.

Superpixel Segmentation: The image is divided into meaningful regions using the SLIC algorithm.

Sparse Saliency:

Saliency is computed as the contrast between superpixels and boundary regions.

Graph-Based Ranking:

A Laplacian matrix is computed, and saliency values are refined via eigen decomposition.

Bayesian Integration:

Sparse and graph-based saliency maps are fused into a unified saliency map.

Visualization: The final saliency map is displayed as a heatmap.

Citation

If you use this code, please cite the original paper:

M. M. Sadiq Fareed et al., "Salient region detection through sparse reconstruction and graph-based ranking," Journal of Visual Communication and Image Representation, 2015.
