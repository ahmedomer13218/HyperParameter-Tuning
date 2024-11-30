# Hyperparameter-Tuning-Regression: Optimizing Regression Models  
This project explores manual and automated **hyperparameter tuning** techniques to optimize regression models, focusing on improving performance and computational efficiency. The methods were applied to a dataset, with experiments ranging from manual tuning to leveraging advanced tools like `keras_tuner`.  

## Table of Contents  
- Overview  
- Features  
- Data Preprocessing  
- Project Structure  
- Installation  
- Usage  
- Contributing  
- License  

### Overview  
This repository focuses on exploring hyperparameter tuning techniques for regression models. Starting with manual tuning, adjustments were made based on model performance, accuracy, and computation time. Automation tools like `keras_tuner` were then introduced to refine the process.  

Dataset: [https://www.kaggle.com/datasets/naiyakhalid/flood-prediction-dataset](#)  

### Features  
#### Manual Tuning    
- Tuned:  
  - Number of layers and neurons  
  - Learning rates: Static, Step Decay, Cyclical Learning Rate (CLR) with 1cycle scheduler, Exponential Decay  
  - Optimizers: `adam`, `nadam`, `SGD`, `rmsprop`  
  - Batch sizes: 16, 32, 64, 128  
  - Activations: `relu`, `tanh`, `selu`  
  - Initializers: `lecun_normal`, `he_normal`, `glorot_normal`  
- **Pruning**: Reduced network size to improve computational efficiency.  

#### Automated Tuning  
- **keras_tuner**: Used RandomSearch and BayesianOptimization to tune:  
  - `batch_size`  
  - `model__optimizer`  
  - `model__activation`  
  - `model__neurons`  

### Evaluation Metrics  
- **Mean Absolute Error (MAE)**  
- **R² Score**  

### Project Structure  
- [RegressionEx_FloodPrediction_ANN.ipynb](./RegressionEx_FloodPrediction_ANN.ipynb)   
- [LICENSE](./LICENSE)  
- [README.md](./README.md)  

### Data Preprocessing  
- Data Loading: Dataset imported for analysis.  
- Splitting: Train-test split for validation.  
- Scaling: Applied transformations for better model performance.  

### Installation  
- Clone this repository:  
```bash  
git clone https://github.com/ahmedomer13218/HyperParameter-Tuning_regression-example.git  

cd HyperParameter-Tuning_regression-example
```
### Usage
- run the notebook

### Contributing
We welcome contributions! If you'd like to contribute, please fork the repository and submit a pull request.

### License
This project is licensed under the MIT License - see the LICENSE file for details.

### 
This repository demonstrates the journey from manual hyperparameter tuning to automated optimization, showcasing practical applications of tuning techniques for regression models. 🎯
