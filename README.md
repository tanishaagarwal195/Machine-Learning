# Machine-Learning
## CAC ASSIGNMENT
### TANISHA AGARWAL
#### 23122041
#### 3MSc DS(A)

## PROBLEM STATEMENT
Here my aim is to explore the effectiveness of Principal Component Analysis (PCA) as a preprocessing technique in combination with Linear Regression for predictive modeling tasks. The dataset under consideration contains a multitude of features, and our goal is to investigate whether dimensionality reduction through PCA enhances the performance of linear regression models while maintaining or even improving interpretability.We have also tried SVR(Support Vector Regrrssion) to see if the accuracy is increased.

Furthermore, we have also divided the prices of diamond into bins and tried SVM(Support Vector Machine) and checked the accuracy then.

## DATASET DESCRIPTION
The dataset comprises-

- price [price in US dollars (326−−18,823)] - TO BE PREDICTED BY OUR MODEL
- carat [weight of the diamond (0.2--5.01)] - NUMERICAL DATA
- cut [quality of the cut (Fair, Good, Very Good, Premium, Ideal)] - CATEGORICAL DATA
- color [diamond colour, from J (worst) to D (best)] - CATEGORICAL DATA
- clarity [a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))] - CATEGORICAL DATA
- x [length in mm (0--10.74)] - NUMERICAL DATA
- y [width in mm (0--58.9)] - NUMERICAL DATA
- z [depth in mm (0--31.8)] - NUMERICAL DATA
- depth [total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)] - NUMERICAL DATA
- table [width of top of diamond relative to widest point (43--95)] - NUMERICAL DATA

# BASIC EDA :
1. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA1.png)
2. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA2.png)
3. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA3.png)
4. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA4.png)
5. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA5.png) 
6. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA6.png) 
7. ![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/outputEDA7.png)

# PCA
![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/PCA-corr.png)

### PCA SCATTER PLOT
![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/scatterplot.png)

## LINEAR REGRESSION
![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/LR.png)

## SVR (AUPPORT VECTOR REGRESSION)
![alt text](https://github.com/tanishaagarwal195/Machine-Learning/blob/main/CAC%20assignment/images/SVR.png)

### Overall Observation:
SVM Classification Performance: The choice of binning strategy for the target variable significantly affects the performance of SVM models. Fewer bins (4 bins) led to better performance, indicating that simpler class structures were easier for the model to learn. 
Regression Performance with PCA: SVR outperformed Linear Regression in the reduced-dimensional space created by PCA. The higher R-squared and lower MSE for SVR suggest it is better suited for capturing complex relationships in the data.
