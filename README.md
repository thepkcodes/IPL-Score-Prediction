# IPL Cricket Score Prediction using Neural Network

## Project Overview

A deep learning model to predict cricket scores in IPL Matches using context and historical data.

## Data Source

IPL Data: The primary dataset used for this model is the [IPL Data](https://github.com/thepkcodes/IPL-Score-Prediction/blob/main/ipl_data.csv) file, containing detailed information about venue, batting team, bowling team, batsman, bowler, runs, wickets, overs, runs and wickets in last 5 overs.

## Tools & Technologies

![Excel](https://img.shields.io/badge/Excel-Spreadsheets-217346?logo=microsoftexcel&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-yellowgreen)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.12%2B-orange) 
![ML](https://img.shields.io/badge/Machine_Learning-8A2BE2?style=flat-square)
![DL](https://img.shields.io/badge/Deep_Learning-9400D3?style=flat-square)

## Libraries Used

- Numpy
- Pandas
- Scikit-Learn
- Matplotlib
- Keras
- Seaborn

## Steps Involved

1. Data Preprocessing
   - Create a new dataframe by dropping some columns
   - split the dataframe into independent variable (X) and dependent variable (y)
   - Applied LabelEncoding to categorical features in X
   - Scale the numerical feature using MinMaxScaler

2. Model Building
   - Used TensorFlow and Keras to build a neural network model.
   - Compiled the model using Huber Loss
   - Train the neural network model using scaled data

3. Model Evaluation
   - Assessing the model's performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R2) score.
   - Iteratively refining the model to achieve better predictive accuracy.

4. Prediction
   - Implementing prediction functionality using the trained model.
   - Creating an interactive prediction interface using ipywidgets for selecting venue, batting team, bowling team, batsman, and bowler.

## Outputs

After experimenting with various neural network architectures and model configurations, the final model achieved the Mean Absolute Error on the test dataset:

Mean Absolute Error (MAE): 12.95

This metric indicate that the model is able to predict IPL scores with a high degree of accuracy.

![image](https://github.com/user-attachments/assets/a814b4c1-e66b-4f07-bbd9-35bae7370c14)

## Installation

1. Clone repository
```bash
git clone https://github.com/thepkcodes/IPL-Score-Prediction.git
cd IPL-Score-Prediction
```

2. Install Dependencies
```bash
pip install -r requirements.txt
```

3. Enable Jupyter Widgets
```bash
jupyter nbextension enable --py widgetsnbextension
```

## Usage

1. Start Jupyter Notebook:
```bash
jupyter notebook
```
2. Open IPL_Score_Prediction.ipynb

3. Use interactive widgets to input match parameters
   - Select venue
   - Choose batting/bowling teams
   - Enter current match status
   - Input recent performance metrics
   - Click "Predict Score" to get instant prediction

![image](https://github.com/user-attachments/assets/1dc77443-6c1f-4296-b803-b9f5314c9e68)

## License

Acknowledgments
TensorFlow/Keras team

Scikit-learn developers

IPL dataset providers
