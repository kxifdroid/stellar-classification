# Stellar Classification using SDSS DR18 Dataset
### Collab link (anyone can view): https://colab.research.google.com/drive/1B1nq-eCWXYdpu4jr3FvDcylRI3PaDB--?usp=sharing

### All images are uploded in the images folder in repo

A machine learning pipeline for classifying celestial objects using data from the Sloan Digital Sky Survey (SDSS) Data Release 18.

## Background

The Sloan Digital Sky Survey (SDSS) is one of the most comprehensive astronomical surveys, providing detailed imaging and spectroscopic data for millions of celestial objects. Accurate classification of stars, galaxies, and quasars is essential for large-scale astronomical research and understanding the structure of the universe.

Machine learning techniques enable automated classification of astronomical objects at scale, reducing manual effort while maintaining high predictive performance.

## Dataset
Also uploaded in the github

Dataset Name: SDSS DR18 Astronomical Objects Dataset

Source:
https://www.sdss.org/dr18/

Number of Samples: 100000

Feature	Description:
u	Ultraviolet magnitude
g	Green magnitude
r	Red magnitude
i	Near-infrared magnitude
z	Infrared magnitude
redshift	Redshift value
ra	Right Ascension
dec	Declination
Additional engineered features	Derived during preprocessing

Target Classes:

Star
Galaxy
Quasar (QSO)
Project Structure
stellar-classification/
│
├── stellar_classification.ipynb
├── README.md
├── requirements.txt
└── data/
    └── sdss_dr18.csv
Files
stellar_classification.ipynb — Complete data analysis, preprocessing, model training, and evaluation pipeline.
README.md — Project documentation.
requirements.txt — Python dependencies required to run the project.

## Setup Instructions
1. Clone the Repository
git clone https://github.com/your-username/stellar-classification.git
cd stellar-classification
2. Install Dependencies

Create a virtual environment (recommended):

python -m venv venv

Activate it:

Windows

venv\Scripts\activate

Linux / macOS

source venv/bin/activate

Install required packages:

pip install -r requirements.txt

Required libraries:

pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
astropy
3. Run the Notebook

Launch Jupyter Notebook:

jupyter notebook

Open:

stellar_classification.ipynb

Run all cells sequentially to reproduce the results.

## Results Summary
Metric	Value
Accuracy	TBD
Macro F1 Score	TBD
Recall (Star)	TBD
Recall (Galaxy)	TBD
Recall (Quasar)	TBD
Key Findings
Photometric magnitudes (u, g, r, i, z) provide strong discriminatory power for distinguishing between stellar and extragalactic objects.
Redshift is among the most influential features for separating galaxies and quasars from stars.
Ensemble learning models such as XGBoost effectively capture complex feature interactions and achieve superior classification performance.


# Acknowledgements
Sloan Digital Sky Survey (SDSS)
SDSS Data Release 18 Team
Scikit-learn Community
XGBoost Contributors
