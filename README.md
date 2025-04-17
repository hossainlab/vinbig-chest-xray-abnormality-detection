# VinBigData Chest X-ray Abnormalities Detection

This repository provides an implementation of deep learning models for detecting and localizing chest X-ray abnormalities using the **VinBigData** dataset. The goal is to classify and identify up to 14 types of thoracic abnormalities from chest radiographs.

## Dataset

The **VinBigData Chest X-ray** dataset contains labeled chest X-ray images for abnormality detection. The dataset includes bounding box annotations for 14 different abnormal conditions.

My solution use 512px resized dataset. And you have two options.
- Download original dataset (~192 GB) and create resized dataset.
- Or download kaggle public dataset already made (3.59 GB).

### Option 1. Download original dataset and create 1024px resized dataset
Download Original Competition data [on the Kaggle competition page](https://www.kaggle.com/competitions/vinbigdata-chest-xray-abnormalities-detection/). And extract zip file.

```bash
kaggle competitions download -c vinbigdata-chest-xray-abnormalities-detection
unzip vinbigdata-chest-xray-abnormalities-detection.zip -d dataset
```
Create 1024px resized dataset. It will be saved to "dataset-jpg" folder. It takes some hours.

### Option 2. Download kaggle public dataset already made
Alternatively, you can use kaggle public dataset - [VinBigData 512 JPG Dataset](https://www.kaggle.com/datasets/awsaf49/vinbigdata-512-image-dataset)

```bash
kaggle datasets download -d sunghyunjun/vinbigdata-1024-jpg-dataset
unzip vinbigdata-1024-jpg-dataset.zip -d dataset-jpg
```
