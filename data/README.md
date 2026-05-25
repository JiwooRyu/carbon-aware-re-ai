#  Wildfire Prediction Dataset

This directory links to the wildfire satellite image dataset used in this project. Due to storage limits, raw images are not included in this repository.

##  Source
- **Kaggle Dataset:** [Wildfire Prediction Dataset (Satellite Images)](https://www.kaggle.com/datasets/abdelghaniaaba/wildfire-prediction-dataset)

##  Dataset Structure
The dataset contains a total of 42,850 images divided into 2 classes:
- `wildfire`: Satellite images with fire/impacted areas.
- `nowildfire`: Satellite images with safe/clear areas.

To run the code, download the dataset from the link above and extract it into this folder using the following structure:

```text
data/
├── README.md
├── train/
│   ├── wildfire/
│   └── nowildfire/
├── valid/
│   ├── wildfire/
│   └── nowildfire/
└── test/
    ├── wildfire/
    └── nowildfire/
