# :star2:Boston Housing Prices : Predictive Learning with Regularized Regression:star2:

This work contains predictive analysis of Boston Housing Prices dataset, with medv as target variable. The analysis is carried out by using Regularized Linear Regression such as Lasso and Ridge method. This analysis is carried out in R (Rstudio).

![ide](https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=RStudio&logoColor=white)
![kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

Just in case you didn't know. The codes are contained in the .Rmd (Rmarkdown) file, whereas the results and codes are neatly combined in the .html file (knitted version of Rmarkdown). Feel free to download and open it 😃😉.

## Objectives
The data is about predicting housing price (medv) in Boston city. All the features can be grouped into :

- Dependent variable: medv, the median value of owner-occupied homes (in thousands of dollars).
- Structural variables indicating the house characteristics: rm (average number of rooms “in owner units”) and age (proportion of owner-occupied units built prior to 1940).
- Neighborhood variables: crim (crime rate), zn (proportion of residential areas), indus (proportion of non-retail business area), chas (river limitation), tax (cost of public services in each community), ptratio (pupil-teacher ratio), black (the black proportion of population) and lstat (percent of lower status of the population).
- Accesibility variables: dis (distances to five Boston employment centers) and rad (accessibility to radial highways – larger index denotes better accessibility).
- Air pollution variable: nox, the annual concentration of nitrogen oxide (in parts per ten million).

## Libraries
This work was mainly done using tidyverse environment and glmnet to build the ML model. However, i also used another libraries to make plots and do certain calculations such as:

- [tidyverse](https://www.tidyverse.org/)
- [caTools](https://cran.r-project.org/web/packages/caTools/index.html)
- [psych](https://cran.r-project.org/web/packages/psych/index.html)
- [glmnet](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiV1Y7ojqf2AhWpSGwGHcR1AE8QFnoECAIQAQ&url=https%3A%2F%2Fcran.r-project.org%2Fweb%2Fpackages%2Fglmnet%2Fglmnet.pdf&usg=AOvVaw0GU29lnFgP5bkxNNIICceO)
- [car](https://cran.r-project.org/web/packages/car/index.html)

## Result preview
According to my hypotheses, the US Economy Crisis had an impact on house sale activity at the time. As a result, this phenomenon could be linked to why there are houses with large ground living area at such low prices.
![preview](https://user-images.githubusercontent.com/92590596/145586144-61ee3f84-26f2-438d-9634-abe93e6c45e2.png)
According to https://www.investopedia.com/terms/g/great-recession.asp , The Great Recession was the sharp decline in economic activity during the late 2000s. It is considered the most significant downturn since the Great Depression. The term Great Recession applies to both the U.S. recession, officially lasting from December 2007 to June 2009, and the ensuing global recession in 2009. The economic slump began when the U.S. housing market went from boom to bust, and large amounts of mortgage-backed securities (MBS’s) and derivatives lost significant value. In Ames however, we get interesting result that that the prices were stagnant during 2006-2010. These years was surely a nightmare for all real estate inventors because the prices didn’t raise year after year.

## References
Regularization is a method in which a penalty called lambda is added in the Loss Function in order to introduce a bias thus overfitting will not happen. The method also can be divided into 2 methods, Ridge (quadratic lambda) and Lasso (absolute lambda). Meanwhile Lasso method is able to reduce the coefficients of certain variables to be completely zero, the Ridge regression can't. To grasp more comprehensive explanation about this topic, I would recommend some great youtube videos made by StatQuest. Here is the link:

- https://www.youtube.com/watch?v=Q81RR3yKn30&t=458s
- https://www.youtube.com/watch?v=NGf0voTMlcs

