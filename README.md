# Satellite Image Segmentation with U-Net

This project uses a U-Net deep learning model to perform semantic segmentation on satellite images, aiming to classify land-use regions.
![image](https://github.com/user-attachments/assets/61fa5c8c-4aaa-487b-93f9-11576c026eb7)


## Project Structure

### 1. **Data**
   - Multispectral satellite images (RGB, NDVI, slope, elevation) in HDF5 format.
   - Contains images and ground truth segmentation masks.

### 2. **Preprocessing**
   - Images are normalized, and NDVI is calculated from the red and near-infrared bands.
   - Dataset is split into training and validation sets.

### 3. **Model**
   - **U-Net** architecture with encoder-decoder blocks and skip connections.
   - Dropout layers are used to prevent overfitting.

### 4. **Training**
   - Trained on the processed dataset using Dice coefficient loss.
   - Includes visualizations of input images, predicted masks, and ground truth masks.

## Requirements

```bash
pip install pandas numpy h5py glob matplotlib tensorflow scikit-learn
