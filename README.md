# Project Name
This case study is to understand 
- Which variables are significant in predicting the price of a house
- How well those variables describe the price of a house.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

Essentially, the company wants to know:
- Which variables are significant in predicting the price of a house, and
- How well those variables describe the price of a house.

Also, determine the optimal value of lambda for ridge and lasso regression.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
The optimal value of lambda are
- Ridge Regression : 20
- Lasso Regression : 0.001

The r2-score, RSS and MSE on train data is slightly better in Ridge compared to Lasso Regression.
However on test data Lasso is slightly better comapred to Ridge Regression.

Ridge regression considers all features whereas in Lasso Regression it reduces co-efficient of 31 variables to zero thus making the model simpler.

Top 5 predictor variables in Ridge Regression are
| Feature      |  Co-eff |
| -----------  | --------|
| HouseAge     | -0.0690 |
| OverallQual  |  0.0638 |
| GrLivArea    |  0.0619 |
| TotalBsmtSF  |  0.0468 |
| OverallCond  |  0.0414 |

The SalePrice of a house significantly depends on
(-0.0690) * HouseAge + 0.0638 * OverallQual + 0.0619 * GrLivArea + 0.0468 * TotalBsmtSF + 0.0414 * OverallCond

Top 5 predictor variables in Lasso Regression are
| Feature      |  Co-eff |
| -----------  | --------|
| GrLivArea    |  0.1129 |
| HouseAge     | -0.0788 |
| OverallQual  |  0.0699 |
| OverallCond  |  0.0442 |
| TotalBsmtSF  |  0.0431 |

The SalePrice of a house significantly depends on
0.1129 * GrLivArea + (-0.0788) * HouseAge + 0.0699 * OverallQual + 0.0442 * OverallCond + 0.0431 * TotalBsmtSF

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy - version 1.21.5
- pandas - version 1.4.2
- matplotlib - version 3.5.1
- seaborn - version 0.11.2
- sklearn - version 1.1.3

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
This project is done as part of Execution PG on ML & AI from upgrade with partnership with IIITB


## Contact
Created by [@ankitlohiya4] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->