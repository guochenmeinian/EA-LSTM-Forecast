# Electricity consumption prediction using attention-based LSTM model

## Overview
This repository hosts the source code for the research paper "Electricity Consumption Prediction Using Evolutionary Attention-based LSTM Model". The paper presents a novel approach to forecasting electricity consumption, leveraging the capabilities of Long Short-Term Memory (LSTM) networks enhanced with an evolutionary attention mechanism.

## Key Contributions
- **Evolutionary Attention-based LSTM (EA-LSTM):** A LSTM variant equipped with an evolutionary attention mechanism to improve its focus on relevant features within a time series.
- **Competitive Random Search Training:** A unique training methodology inspired by evolutionary computations, designed to optimize the model's attention layer parameters more effectively than traditional gradient-based methods.
- **Empirical Validation:** The EA-LSTM model is rigorously tested against standard machine learning techniques (Lasso Regression, XGBoost, Random Forest) and contemporary deep learning methods (LSTM and GRU).
- **Performance Metrics:** The model's superiority is demonstrated across multiple metrics, including RMSPE, RMSE, MAPE, and MAE.

## Model Description
The EA-LSTM model is crafted to address the limitations of traditional LSTMs in handling time series data with varying degrees of importance across different time steps. By integrating an evolutionary attention layer, the model can adaptively focus on the most relevant sub-window features for effective temporal relationship mining. This approach mimics biological evolution patterns in identifying crucial data points. Therefore, the pattern for importance-based attention sampling can be acquired during temporal relationship mining.

The competitive random search method for training circumvents the pitfalls of partial optimization, common in gradient-based techniques. This innovative training strategy ensures a comprehensive exploration of the optimization space, leading to a more robust and efficient parameter configuration in the attention layer.

## Repository Structure
- `source_code/`: Contains the full source code used for implementing the EA-LSTM model.
- `data/`: Sample datasets used for training and evaluating the model.
- `results/`: Results and comparisons with baseline methods.
- `documentation/`: Additional documentation and guidelines for replicating the experiments.

### Reference
For implementation, I referred to (the author's original code)[https://github.com/bzantium/EA-LSTM].


## The paper has been submitted to **PLOS ONE** and is currently under review (major revision).
