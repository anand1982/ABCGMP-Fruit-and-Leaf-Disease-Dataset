# ABCGMP-Fruit-and-Leaf-Disease-Dataset
# ABCGMP: Multi-Crop Fruit and Leaf Disease Dataset

[![Dataset](https://img.shields.io/badge/Dataset-Mendeley%20Data-orange)](https://doi.org/10.17632/v6p3p7g5z2) 
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

The **ABCGMP** (Apple, Banana, Citrus, Guava, Mango, and Papaya) dataset is a comprehensive multi-crop image repository for plant pathology research. It addresses the challenge of automated disease detection in diverse agricultural environments by providing high-quality images of both **fruits and leaves**.

Dataset Link: https://data.mendeley.com/datasets/fhbvmpcyy2/2

---

## 📊 Dataset Description

The repository contains samples from six economically vital horticultural crops. The dataset preserves real-world symptom diversity, including fungal, bacterial, and viral manifestations such as:
* **Fruit:** Rot, Scab-like lesions, and Necrotic spots.
* **Leaf:** Spots, Blight, Anthracnose, Red Rust, Canker, and Ring Spot.
* **Apple:** Healthy Fruit, Disease Fruit, Healthy Leaf, Black Rot
![Apple Dataset Sample Images](AP.png)

Black rot, caused by the fungus Diplodia seriata, affects the leaves, fruit, and bark of apple trees. On the fruit, it typically appears as a firm, brown-to-black rot originating from the calyx or a wound, often characterized by concentric rings. On leaves, it manifests as small purple spots that evolve into "frog-eye" lesions with a tan center and purple rim.

* **Banana:** Healthy Fruit, Disease Fruit, Healthy Leaf, Cordana
![Banana Dataset Sample Images](BI.png)

Caused by the fungus Cordana musae, this disease primarily attacks the foliage of banana plants. It presents as large, oval-shaped lesions with a distinct grayish-brown center surrounded by bright yellow halos. As the infection progresses, the lesions expand along the leaf margins, significantly reducing the photosynthetic capacity of the plant.

* **Citrus:** Healthy Fruit, Disease Fruit, Healthy Leaf, Canker Leaf
![Citrus Dataset Sample Images](CI.png)


* **Guava:** Healthy Fruit, Disease Fruit, Healthy Leaf, Black Rot
![Guava Dataset Sample Images](GI.png)



* **Mango:** Healthy Fruit, Disease Fruit, Healthy Leaf, Bacterial Canker
![Mango Dataset Sample Images](MI.png)


* **Papaya:** Healthy Fruit, Disease Fruit, Healthy Leaf, Ring Spot
![Papaya Dataset Sample Images](PI.png)

### 📝 Disease Overview
The dataset covers a wide spectrum of plant pathologies, as summarized below:

| Crop | Disease | Part | Description |
| :--- | :--- | :--- | :--- |
| **Apple** | Black Rot | Leaf/Fruit | Brown rot with concentric rings; purple-rimmed leaf spots. |
| **Banana** | Cordana | Leaf | Large oval lesions with distinct yellow halos. |
| **Citrus** | Canker | Leaf/Fruit | Contagious bacterial corky lesions and necrotic spots. |
| **Guava** | Red Rust | Leaf | Algal-based rusty colored velvety circular spots. |
| **Mango** | Bacterial Canker | Leaf/Fruit | Water-soaked angular spots and star-shaped fruit lesions. |
| **Papaya** | Ring Spot | Leaf/Fruit | Viral mosaic patterns and characteristic fruit rings. |

### Data Distribution by Crop and Class

| S.No | Crop | Class | Images | Crop | Class | Images |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | **Apple** | Healthy Leaf | 2008 | **Guava** | Red Rust | 90 |
| 2 | **Apple** | Black Rot | 1987 | **Guava** | Healthy Leaf | 150 |
| 3 | **Apple** | Healthy Fruit | 301 | **Guava** | Disease Fruit | 160 |
| 4 | **Apple** | Disease Fruit | 286 | **Guava** | Healthy Fruit | 50 |
| 5 | **Banana** | Cordana | 739 | **Mango** | Bacterial Canker | 404 |
| 6 | **Banana** | Healthy Leaf | 535 | **Mango** | Healthy Leaf | 308 |
| 7 | **Banana** | Healthy Fruit | 133 | **Mango** | Disease Fruit | 213 |
| 8 | **Banana** | Disease Fruit | 74 | **Mango** | Healthy Fruit | 348 |
| 9 | **Citrus** | Canker Leaf | 210 | **Papaya** | Ring Spot | 717 |
| 10 | **Citrus** | Healthy Leaf | 192 | **Papaya** | Healthy Leaf | 298 |
| 11 | **Citrus** | Disease Fruit | 158 | **Papaya** | Disease Fruit | 127 |
| 12 | **Citrus** | Healthy Fruit | 190 | **Papaya** | Healthy Fruit | 143 |

### 🌍 Data Sourcing
To ensure robustness against variations in lighting and background, images were sourced as follows:
- **50%:** Direct field acquisition (Uncontrolled conditions).
- **16%:** Crowdsourced from farmers (Smartphone cameras).
- **20%:** Public benchmark datasets.
- **14%:** Verified online agricultural repositories.

---

## 💻 Deep Learning Setup

For training models (such as MDTACNet) on **Kaggle** or **Google Colab**, follow these requirements.

### Hardware Requirements
- **GPU:** NVIDIA Tesla T4, P100, or K80 (Minimum 8GB VRAM).
- **RAM:** 12GB+ (High RAM mode recommended for large Transformer-based models).

### Software & Libraries
```bash
pip install tensorflow torch torchvision opencv-python matplotlib scikit-learn
