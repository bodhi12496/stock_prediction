
# PREDICTING STOCK PRICE USING LSTM

This report presents our project on forecasting stock prices using a feature fusion
LSTM-CNN model based on the research paper "Forecasting Stock Prices with a Feature
Fusion LSTM-CNN Model Using Different Representations of the Same Data." We aim to
replicate the paper's model and explore the impact of different data representations on
stock price prediction. 


## Tech Stack

Python , LSTM , Sc-CNN model , Tensorflow , Keras 



##  Results obtained on implementing the models:

 LSTM Model:
-  Loss: 1.2461
- MAPE: 5.43%
- RMSE: 1.1163

SC-CNN Model:
- Loss: 0.0416
- MAPE: 5.44%
- RMSE: 0.2040

Fusion Model:
- Loss: 39900.3945

## Recommendations to improve the model performance:

- Investigate and address issues causing high loss in the Fusion model.
- Explore alternative fusion techniques and architectures.
- Consider additional feature engineering and preprocessing steps for improved model performance.

Few modifications performed on the fusion model:
- Additional Dense Layers: The code adds more dense layers to the Fusion model, allowing it to capture more complex relationships.
- Learning Rate Adjustment: Lowering the learning rate can sometimes help the model converge more effectively and avoid overshooting the minimum.
- Different Activation Functions: Adjusting activation functions in the additional layers might improve the model's ability to capture non-linear patterns.
- Training with Adjusted Parameters: The model is then trained with the adjusted architecture and hyperparameters

## Results after fine tuning fusion model:
The following are the values of the fusion loss obtained on the different representations
with and without performing modifications
Without Refinement:
- Fusion Model on Stock and Linebar: 12075.2832
- Fusion Model on Stock and F-linebar: 12075.2832
- Fusion Model on Candlebar: 12075.2832
- Overall Fusion Model: 39900.3945
With Refinement :
- Fusion Model on Stock and Linebar: 9658.22
- Fusion Model on Stock and F-linebar: 9658.22
- Fusion Model on Candlebar: 9658.22
- Overall Fusion Model: 31920.3156







