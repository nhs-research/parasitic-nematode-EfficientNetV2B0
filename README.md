# Short overview
This repository contains the Google Colab file used to train a parasitic nematode identification model is based on <b>EfficientNetV2B0</b> using a combination of three different optimizers (Adam, SGD, dan RMSProp) and several data augmentation with image transformations, such as image flip, blurring, noise addition, brightness, and contrast adjustment. 

The dataset used can be accessed <a href='https://data.mendeley.com/datasets/cck8yxj3xw/1'>here</a>

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
@article{https://doi.org/10.1016/j.aiia.2022.12.002,
  title={Deep learning models for automatic identification of plant-parasitic nematode},
  author={Nabila Husna Shabrina, Ryukin Aranta Lika, Siwi Indarti },
  journal={Artificial Intelligence in Agriculture},
  year={2023}
}
