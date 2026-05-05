# Lab 9 - Morphological Operations

A Python lab exploring basic morphological operations in image processing using OpenCV.

## Operations Covered
- **Erosion** – shrinks object boundaries
- **Dilation** – expands object boundaries
- **Opening** – removes small noise (erode → dilate)
- **Closing** – fills small holes (dilate → erode)
- **Boundary Extraction** – detects object edges (gradient, internal, external)

## Requirements
```bash
pip install opencv-python numpy matplotlib
```

## Image Files Needed
Put these images in the same folder as the notebook:
- `Erosion.jpg`
- `Open_Closing.jpg`
- `Opening2.jpg`
- `BoundaryExtraction.jpg`

## How to Run
Open the notebook in Jupyter and run the cells from top to bottom.
```bash
jupyter notebook Lab_9_Morphological_Operations.ipynb
```