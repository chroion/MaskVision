# Novel Open Photomask Benchmark and Efficient Anomaly Detection for Semiconductor Applications 

This repository provides a **large-scale Photomask dataset** intended for **anomaly detection research** in semiconductor manufacturing. The dataset features high-resolution images reflecting real-world photomask patterns, including both normal and defect samples. By sharing these images, we aim to support the development of methods that can handle **large volumes** of **high-resolution** data under **industrial** conditions.

## Table of Contents

- [Overview](#overview)
- [Dataset Structure](#dataset-structure)
- [Download](#download)
- [Citation](#citation)

------

## Overview

In semiconductor lithography, photomasks serve as templates to transfer intricate circuit patterns onto silicon wafers. Even small or **weak defects** on a photomask can lead to significant yield loss in high-volume production. This dataset contains **high-resolution** images capturing these patterns and includes both artificially introduced defects (e.g., dust or micro-scratches) and naturally occurring anomalies.

**Key Features:**

- **High Resolution:** Raw images are captured at up to 172,000×249,000 pixels, then subdivided into smaller patches (e.g., 128×128) for manageability.
- **Diverse Defect Types:** Ranging from dust, scratches, and contamination to subtle line-width deviations.
- **Industrial-Scale Complexity:** Reflects real-world manufacturing challenges, such as repetitive patterns and large data volumes.

------

## Dataset Structure

Below is an example directory layout after downloading the dataset:

    photomask_dataset/
    ├── train/
    │   └── good/
    │       ├── 0001.png
    │       ├── 0002.png
    │       └── ...
    ├── test/
    │   ├── defect/
    │   │   ├── 0001.png
    │   │   ├── 0002.png
    │   │   └── ...
    │   └── good/
    │       ├── 1412.png
    │       ├── 1413.png
    │       └── ...
    ├── ground_truth/
    │   └── defect/
    │       ├── 0001_mask.png
    │       ├── 0002_mask.png
    │       └── ...
    └── README.md

- **train/good/**: Normal patches used for training.
- **test/good/**: Normal patches for testing.
- **test/defect/**: Defect patches for testing and evaluation.
- **test/ground_truth/**: Ground truth image for testing and evaluation.

The exact directory structure may vary depending on how you choose to organize normal and defect images.

## Download

Due to the **large size** of the dataset, we provide two download options:

1. **Full Dataset:**
   - High-resolution image patches suitable for comprehensive training and evaluation.
   - Recommended for researchers focusing on large-scale industrial scenarios.
2. **Sample Subset:**
   - A smaller collection of representative images (both normal and defect) for quick prototyping or demonstration.
   - Ideal for users with limited storage or computational resources.

**Download Links**

- Full Dataset Link (TBD)
- [Sample Subset Link](https://www.kaggle.com/datasets/chroion/photomask-subset/data?select=test)

## Citation

If you use this dataset in your research, please cite:

**TBD**
