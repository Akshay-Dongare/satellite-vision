# Satellite Vision: Comparing CNN and Vision Transformer Approaches for Land Use Classification

## Team 37
1. Akshay Dongare
2. Anish Mulay
3. Ayush Gala


## Motivation and Problem Statement
Satellite imagery analysis plays a crucial role in various real-world applications including urban planning, environmental monitoring, and disaster response. While Convolutional Neural Networks (CNNs) have traditionally dominated image classification tasks, Vision Transformers (ViTs) have emerged as a powerful alternative, demonstrating superior performance in capturing global spatial relationships through self-attention mechanisms.

This project aims to compare the effectiveness of CNNs and ViTs in classifying land use patterns from satellite imagery, providing insights into which architecture might be better suited for specific remote sensing tasks.

## Datasets
We utilize two prominent satellite imagery datasets:

1. [EuroSAT](https://zenodo.org/records/7711810#.ZAm3k-zMKEA)
   - 64x64 pixel RGB images
   - Mean pixel intensity: 103.80
   - Standard deviation: 12.19
   - Pixel value range: 82-204

2. [UC Merced Land Use Dataset](http://weegee.vision.ucmerced.edu/datasets/landuse.html)
   - 256x256 pixel RGB images
   - Mean pixel intensity: 114.90
   - Standard deviation: 22.39
   - Pixel value range: 33-253

## Exploratory Data Analysis (EDA)
Our EDA reveals several key insights about the datasets:

1. **Image Characteristics**
   - Significant resolution differences between datasets (64x64 vs 256x256)
   - Different pixel intensity distributions and ranges
   - UC Merced shows higher variance in pixel values

2. **Spectral Analysis**
   - RGB channel distributions across land use classes
   - Analysis of color patterns specific to different land use types

## Implementation
The project implements and compares:
- CNN-based architecture
- Vision Transformer (ViT) architecture

## Project Structure
```python
satellite-vision/
├── EuroSAT_RGB/         # EuroSAT dataset
├── UCMerced_LandUse/    # UC Merced dataset
├── eda.ipynb            # Exploratory Data Analysis notebook
└── README.md
```

## Requirements
- Python 3.x
- PyTorch
- NumPy
- Pandas
- Matplotlib
- OpenCV

## References
1. Helber, P., et al. (2019). EuroSAT: A Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover Classification. IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing.
2. Yang, Y., & Newsam, S. (2010). Bag-of-visual-words and spatial extensions for land-use classification. ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems.
