# Short overview
This repository contains the Google Colab file used to train a parasitic nematode identification model is based on <b>EfficientNetV2B0</b> using a combination of three different optimizers (Adam, SGD, dan RMSProp) and several data augmentation with image transformations, such as image flip, blurring, noise addition, brightness, and contrast adjustment. 

The dataset used can be accessed <a href='https://data.mendeley.com/datasets/cck8yxj3xw/1'>here</a>

# Dataset Specification
* Image size: 1280 x 1024 pixel 
* Data format: .jpg 
* Number of images: 1016 images 
* Class: Xiphinema, Meloidogyne, Trichodorus, Hirschmanniella, Hoplolaimus, Criconemoides, Hemicycliophora, Radopholus, Pratylenchus, Criconema, and Helicotylenchus
* Data source location: Central Java and Yogyakarta, Indonesia

# Dataset Structure
Class distribution:
1. Xiphinema: 85 images
2. Meloidogyne: 211 images
3. Trichodorus: 44 images
4. Hirschmanniella: 130 images
5. Hoplolaimus: 151 images
6. Criconemoides: 4 images
7. Hemicycliophora: 6 images
8. Radopholus: 31 images
9. Pratylenchus: 116 images
10. Criconema: 103 images
11. Helicotylenchus: 135 images

# Installation and Setup
It's recommended to use <b>Google Colab</b> for this notebook, by following these steps:
1. Duplicate the notebook
2. Download the dataset and upload it to Google Drive
3. Set up notebook secrets consisted of:
   * CHECKPOINT_PATH
   * DATASET_NAME
   * ZIP_PATH
4. Run the code

# Results & Findings
* The model trained with RMSProp and brightness augmentation give the best result of 97.94%
  
# Citation
If you use this project or its resources, please cite the following:

**Research Paper**  
Shabrina, N. H., Lika, R. A., & Indarti, S. (2023). Deep learning models for automatic identification of plant-parasitic nematode. *Artificial Intelligence in Agriculture*, 7, 1–12. [https://doi.org/10.1016/j.aiia.2022.12.002](https://doi.org/10.1016/j.aiia.2022.12.002)

**Dataset**  
Indarti, S., Shabrina, N. H., & Maharani, R. (2025). Microscopic Image Dataset of Plant-Parasitic Nematodes. *Mendeley Data*, V1. [https://doi.org/10.17632/cck8yxj3xw.1](https://doi.org/10.17632/cck8yxj3xw.1)

```plaintext
@article{Shabrina2023,
  title   = {Deep learning models for automatic identification of plant-parasitic nematode},
  author  = {Shabrina, Nabila Husna and Lika, Ryukin Aranta and Indarti, Siwi},
  journal = {Artificial Intelligence in Agriculture},
  volume  = {7},
  pages   = {1--12},
  year    = {2023},
  doi     = {10.1016/j.aiia.2022.12.002}
}

@dataset{Indarti2025,
  title    = {Microscopic Image Dataset of Plant-Parasitic Nematodes},
  author   = {Indarti, Siwi and Shabrina, Nabila Husna and Maharani, Rina},
  year     = {2025},
  publisher= {Mendeley Data},
  version  = {1},
  doi      = {10.17632/cck8yxj3xw.1}
}
