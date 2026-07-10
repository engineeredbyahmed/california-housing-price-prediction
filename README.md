{\rtf1\ansi\ansicpg1252\cocoartf2870
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # California Housing Price Prediction\
\
This project explores different approaches for predicting house prices in California using the California Housing dataset from the 1990 U.S. Census.\
\
Rather than focusing on a single model, the objective was to compare several machine learning techniques and understand **why some models perform better than others** when dealing with nonlinear housing data.\
\
---\
\
## Models Evaluated\
\
- Linear Regression\
- Random Forest Regression\
- Support Vector Regression (SVR)\
- Multilayer Perceptron (MLP)\
\
---\
\
## Results\
\
| Model | R\'b2 | RMSE |\
|------|------:|------:|\
| Random Forest | **0.83** | **47,074** |\
| Linear Regression | 0.65 | 67,386 |\
| MLP | 0.64 | 68,301 |\
| Support Vector Regression | 0.61 | 70,930 |\
\
Random Forest achieved the strongest overall performance, while the MLP produced results very similar to Linear Regression despite its higher computational complexity.\
\
One interesting outcome was that increasing model complexity did **not** necessarily improve predictive performance.\
\
---\
\
## What this project includes\
\
- Data preprocessing\
- Exploratory data analysis\
- Feature engineering\
- K-Means clustering\
- Principal Component Analysis (PCA)\
- Hyperparameter tuning\
- Learning curve analysis\
- Model comparison\
- Feature importance analysis\
\
---\
\
## Key Findings\
\
- Median income was the strongest predictor of house value.\
- Geographic location played a major role in price variation.\
- Random Forest handled nonlinear relationships considerably better than the other evaluated models.\
- Prediction errors increased for high-value houses because the dataset is capped at \\$500,000.\
\
---\
\
## Technologies\
\
- Python\
- Pandas\
- NumPy\
- Scikit-learn\
- TensorFlow / Keras\
- Matplotlib\
- Seaborn\
- Jupyter Notebook\
\
---\
\
## Dataset\
\
This project uses the **California Housing Dataset**, which is publicly available through Scikit-learn.\
\
The dataset is therefore **not included** in this repository.\
\
```python\
from sklearn.datasets import fetch_california_housing\
```\
\
---\
\
## Repository Structure\
\
```\
.\
\uc0\u9500 \u9472 \u9472  notebooks\
\uc0\u9500 \u9472 \u9472  images\
\uc0\u9500 \u9472 \u9472  README.md\
\uc0\u9500 \u9472 \u9472  requirements.txt\
\uc0\u9492 \u9472 \u9472  LICENSE\
```\
\
---\
\
## Future Improvements\
\
There are several directions that could improve performance:\
\
- Incorporate additional socioeconomic variables\
- Explore ensemble or hybrid models\
- Apply automated hyperparameter optimization\
- Evaluate gradient boosting methods such as XGBoost or LightGBM\
\
---\
\
## Author\
\
Ahmed Al Dulaim\
\
MSc Data Science \'97 University of Exeter\
Biomedical Engineer}