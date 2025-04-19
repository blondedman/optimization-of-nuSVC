# optimization of nuSVC

## Dataset Used:
**HTRU2** <br>
- [https://archive.ics.uci.edu/dataset/372/htru2](https://archive.ics.uci.edu/dataset/372/htru2) <br>
- pulsar candidates collected during the HTRU survey <br>
- pulsars are a type of star, of considerable scientific interest

## Methodology Used:
- **Data Preprocessing**  
   - target variable is separated from the feature set
   - 70-30 split is done over 10 samples which are to be evaluated separately
   - features are standardized using StandardScaler to improve model performance

- **Model Selection**
   - **nu Support Vector Classifier (nuSVC)** classifier is selected from sklearn.svm

- **Parameter Optimization**
   - randomized parameter optimization is done using a fitness function
   - cross-validation is used to ensure the generalizability of the model

- **Model Evaluation**
   - accuracy score is used as the primary performance metric
     
## Final Results:
![results](https://github.com/blondedman/optimization-of-nuSVC/blob/main/nuSVC-results.png?raw=true)

## Convergence Graph
![convergence](https://github.com/blondedman/optimization-of-nuSVC/blob/main/nuSVC-convergence.png?raw=true)
