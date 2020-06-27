# Quant Project on Factor Investment with A-Stock
## Description
This is a quant project on all the stock listed in A-stock market from January 2007 to August 2018 with 44 stock selection factors covering fundamental, price-volume, and sentiment. <br />

To build a new synthetic factor, 3 supervised learning methods are applied: <br />
1. Regression with Regularization Technique (Ridge & Lasso) <br />
2. Support Vector Machine (Support Vector Regression) <br />
3. Random Forests (Random Forests Regression) <br />

## Files Included
### Jupyter Notebook
1.SVR.ipynb: <br />
2.Random Forest.ipynb: <br />
3.Ridge.ipynb: <br />
4.Lasso_ tradingSimulation.ipynb: 
The content at the beginning of this file is about Lasso model building and cross-validation.
The Latter part is for More Considerations in the Trading Simulation.
The Latter part is for More Considerations in the Trading Simulation. <br />
-Differentiated Weights
-Trading Feasibility
-Shorting Constraints -Trading Cost


### Python Script
1.backtestlite.py: This file is used to simulate a Long-Short strategy with the prediction information generated by the supervised learning methods mentioned above.  <br />
2.backtestlite_weight.py: The method in the file "backtestlite.py" called getQuantileWeight has been modified to reflect Differentiated Weights.  <br />
3.Backtestlite_tc.py: 2 more methods are added (cal_net_value_tc, cal_ls_rtn_tc) to reflect the net value and net value change rate on a LS-strategy portfolio after transaction costs. <br />
4.helper.py: This file is used for performance visulization and key performance metrics calculation. <br />
5.helper_tc.py: The code for wealth curve plotting is modified to plot the net value and the key metrics (i.e., IR, Drawdown...) after transaction costs.
