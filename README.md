# LitNet Research Project

This repository contains a collection of medical image segmentation experiments based on LitNet and U-Net variants for different datasets.

## Project overview

The workspace is organized into separate dataset-specific folders:

- `Kevasir dataset/` – segmentation experiments for gastrointestinal polyp images
- `Lung_CT/` – lung CT nodule segmentation experiments
- `Wound Dataset/` – wound segmentation experiments
- `Paper/` – research paper or related documentation

Each folder includes:

- Jupyter notebooks for model training and inference
- Trained `.h5` model checkpoints
- Dataset folders with training and testing images/masks
- Result folders for saved predictions or evaluation outputs

## Models included

The project evaluates several segmentation architectures and activation variants, including:

- LitNet
- U-Net with ReLU
- U-Net with LeakyReLU
- LitUNet with DLU

These models are stored as checkpoint files such as:

- `best_model_LitUNet_DLU_run1.h5`
- `best_model_UNet_ReLU_run1.h5`
- `best_model_UNet_LeakyReLU_run1.h5`

## Dataset structure

Each dataset folder contains image and mask splits, for example:

- `images/` and `masks/`
- `t_images/` and `t_masks/`
- `train_images/`, `train_masks/`, `test_images/`, `test_masks/`

## Requirements

To run the notebooks, install the following:

- Python 3.9+
- TensorFlow / Keras
- NumPy
- OpenCV
- Matplotlib
- scikit-image
- Jupyter Notebook or JupyterLab

Example installation:

```bash
pip install tensorflow numpy opencv-python matplotlib scikit-image jupyter
```

## How to use

1. Open the dataset folder you want to study.
2. Launch the relevant `.ipynb` notebook in Jupyter.
3. Run the cells in order to:
   - load the dataset
   - preprocess images and masks
   - train or evaluate the model
   - generate segmentation results

## Notes

- Model weights are saved in HDF5 format (`.h5`).
- Outputs and result visualizations are stored in each dataset's `Results/` or `results/` folder.
- The notebooks are the primary entry points for reproduction and experimentation.

## Repository status

This project is organized as a research codebase for medical image segmentation experiments and is primarily intended for academic and experimental use.
