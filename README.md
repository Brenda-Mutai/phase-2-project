ANALYSIS OF KING COUNTY HOUSE

![Alt text](20230709_103354-2.jpg)

OVERVIEW

The king county house data analyses houses in order to make recommendations to a real estate agency.The data has information about fixed aspects of the houses that includes the location, the year the house wa built,features that can be modified in the house.The various characteristics of the homes will determine various variables such as the house sqft, number of floors, number of bathrooms were used in the linear regression analysis to find the highest correlation of the features.From this data we will be able to maximize on the houses resale values.

BUSINESS PROBLEM

The real estate company is interested in doing renovations to improve the home values in King County. Hence to assist the King County real estate agency we will have to understand the market value of the local houses while comparing others in order to recommend profitable renovations to King County clients.

DATA UNDERSTANDING

The data provided  has different aspects of the homes. These comprises the year they were constructed, the cost of the home, the number of bedrooms, bathrooms and floors, among other essential details of the house such the views.

DATA ANALYSIS AND MODELING

We will analyse the data using various variables because the purpose of this study is to find ways in which King County houses might be restored or upgraded in order to maximise on the resale values.
The price will be the dependent variable while all the other features like bedrooms, bathrooms,sqft living, floors will the independent variables.

![Alt text](image.png)

Baseline Model
          OLS Regression Results                            
==============================================================================
Dep. Variable:                  price   R-squared:                       0.492
Model:                            OLS   Adj. R-squared:                  0.492
Method:                 Least Squares   F-statistic:                 2.087e+04
Date:                Sat, 08 Jul 2023   Prob (F-statistic):               0.00
Time:                        22:41:42   Log-Likelihood:            -2.9912e+05
No. Observations:               21534   AIC:                         5.982e+05
Df Residuals:                   21532   BIC:                         5.983e+05
Df Model:                           1                                         
Covariance Type:            nonrobust                   
===============================================================================
                  coef    std err          t      P>|t|      [0.025      0.975]
-------------------------------------------------------------------------------
const        5.401e+05   1777.605    303.812      0.000    5.37e+05    5.44e+05
sqft_living   279.9321      1.938    144.473      0.000     276.134     283.730
==============================================================================
Omnibus:                    14582.265   Durbin-Watson:                   1.981
Prob(Omnibus):                  0.000   Jarque-Bera (JB):           516142.289
Skew:                           2.781   Prob(JB):                         0.00
Kurtosis:                      26.331   Cond. No.                         917.
==============================================================================

Notes:
[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.

Baseline Model Interpretation and Visualization

 OLS regression results for sqft living variable indicates that for each additional unit the price is like to increase by $279.9321 in price.
The p values are statically significant with the coefficient estimate and intercept.
![Alt text](image-1.png)

Final Model results
OLS Regression Results                            
==============================================================================
Dep. Variable:                  price   R-squared:                       0.530
Model:                            OLS   Adj. R-squared:                  0.530
Method:                 Least Squares   F-statistic:                     8095.
Date:                Sat, 08 Jul 2023   Prob (F-statistic):               0.00
Time:                        23:28:19   Log-Likelihood:            -2.9829e+05
No. Observations:               21534   AIC:                         5.966e+05
Df Residuals:                   21530   BIC:                         5.966e+05
Df Model:                           3                                         
Covariance Type:            nonrobust                                         
====================================================================================
                       coef    std err          t      P>|t|      [0.025      0.975]
------------------------------------------------------------------------------------
const             5.096e+05   1909.209    266.894      0.000    5.06e+05    5.13e+05
sqft_living        243.6022      3.000     81.194      0.000     237.722     249.483
bathrooms         6190.2220   3406.363      1.817      0.069    -486.503    1.29e+04
interaction_term    58.8343      1.414     41.600      0.000      56.062      61.606
==============================================================================
Omnibus:                    10334.375   Durbin-Watson:                   1.986
Prob(Omnibus):                  0.000   Jarque-Bera (JB):           384803.685
Skew:                           1.647   Prob(JB):                         0.00
Kurtosis:                      23.445   Cond. No.                     2.96e+03
==============================================================================

Notes:
[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.
[2] The condition number is large, 2.96e+03. This might indicate that there are
strong multicollinearity or other numerical problems.

![Alt text](image-3.png)

RECOMMENDATIONS

King County real estate agency should consider in maximizing on their property values by icluding extra amenities such as having excellent house views.

Homeowners should also consider elevating the house values by improving amenities such as the bathroons and bedroons.King County homeselllers can use the regression models to determine a given property  compared to a given home. Improved amenities such as bathrooms and bedrooms have a great impact on the house value.

I would also advise King County real estate agency to advise homeowners in considering more square foot in their house when building or renovating.

The linear Regression indicates the impact on the house sale price by the home owners doing renovations and the type of renovations that would boost the market of the homes.

NEXT STEPS

King County should consider looking at the most recent trends in the house market. Conducting a market research through media study on what is modern in order to gain different insights and maximize on the sale.
