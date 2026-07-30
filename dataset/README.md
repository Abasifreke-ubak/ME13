# Dataset — Potato Early Blight vs Late Blight

## Source

**Kaggle:** [PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset)
by **Abdallah Ali**

## Brief Description

The PlantVillage dataset contains leaf images for 38 plant disease categories across
multiple crops. The dataset provides three image variants per class: `color`, `grayscale`,
and `segmented`. For this project only the **`color/`** variant is used, and only the
**`Potato___Early_blight`** and **`Potato___Late_blight`** classes are selected — the
healthy potato class and all other crops are excluded. Images are provided as flat class
folders with no pre-made splits; the notebook builds a stratified **70 / 15 / 15**
train / val / test split at runtime using a fixed seed (42). All images are resized to
**224 × 224** pixels during loading. For full details on collection method and licensing
refer to the dataset page linked above.

## Structure (used subset, after runtime split)

```
potato_split/
├── train/
│   ├── Early_Blight/
│   └── Late_Blight/
├── val/
│   ├── Early_Blight/
│   └── Late_Blight/
└── test/
    ├── Early_Blight/
    └── Late_Blight/
```
