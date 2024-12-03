# Kidney Stone Detection Using Image Processing Techniques

## Overview
This project focuses on detecting kidney stones from ultrasound images using various image processing techniques. The objective is to provide an efficient and accurate method for early diagnosis of kidney stones, leveraging acoustic shadows observed in ultrasound images.

## Features
- **Image Preprocessing**: Removal of speckle noise and isolation of the region of interest using Otsu Thresholding.  
- **Image Enhancement**: Noise reduction using Gaussian and Median filters.  
- **Image Segmentation**: Detection of kidney stone regions using morphological operations like dilation and erosion.  
- **Result Interpretation**: Identification of stones and generation of a clean black image for cases without stones.  

## Technologies Used
- **Programming Language**: Python  
- **Libraries**: OpenCV, NumPy, Matplotlib, Scikit-image  



## Getting Started

### Prerequisites
- Python 3.8 or later  
- OpenCV  
- NumPy  
- Matplotlib  
- Scikit-image  

### Directory Structure
kidney-stone-detection/
├── data/                  # Contains input ultrasound images
├── src/                   # Source code files
├── results/               # Output images and results
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation

## Methodology
1. **Image Preprocessing**:  
   - Noise removal using Otsu Thresholding.  
   - Filling foreground regions to isolate the area of interest.  
2. **Image Enhancement**:  
   - Applied Gaussian blur to reduce speckle noise.  
   - Used Median filtering to handle salt-and-pepper noise.  
3. **Image Segmentation**:  
   - Morphological operations (Dilation and Erosion) to detect and highlight stone regions.  
4. **Result Generation**:  
   - Highlighted kidney stone regions in ultrasound images.  
   - Produced black images for cases with no stones.

## Dataset
The project uses ultrasound images of kidneys, with and without stones, as the input dataset. Ensure that the dataset is placed in the `data/` directory before running the program.


## Results
### Image with a stone:
![Image with Stone](results/image_with_stone.png)

### Image without a stone:
![Image without Stone](results/image_without_stone.png)

