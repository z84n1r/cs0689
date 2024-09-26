java c
Nonlinear econometrics for finance
HOMEWORK 1
(Review of linear econometrics and review of methods)
Problem 1 (Linear econometrics.) (60 points) Household finance is a growing field in finance. In this homework you will study medical household expenditures, using data from a developing region in Vietnam. The dataset in the file vietnam.csv contains the following information:
• sex: gender of household head (male, female)
• age: age of household head
• education: years of schooling of household head
• farm: does the household engage in farming?
• urban: is the household in an urban area?
• hhsize: number of people in the household
• totalexp: household total expenditure
• medexp: household medical expenditure
• community: community where the household lives
Given this information, you need to perform. linear regression in Python to understand the drivers of medical expenditures.
(1) (3 points) Generate an histogram of the medical expenditures and com-pute descriptive statistics (mean, median, standard deviation, mini-mum, maximum). Is the distribution symmetric? Provide an economic justification for your answer: what could explain the lack (or presence) of symmetry?
(2) (3 points) Take a logarithmic transformation of the medical expendi-tures. Now, plot the histogram of the log-expenditure. What do you notice? How would you explain the change?
Begin by excluding all categorical variables (sex, farm, urban and commu-nity).
(3) (6 points) Transform. total expenditure into logarithms and run a re-gression of the log medical expenditures on the non-categorical ex-planatory variables (with total expenditures in log). The model you are estimating is:
log(medexpi) = θ0 + θ1agei + θ2educationi + θ3hhsizei + θ4 log(totalexpi) + εi,
where εiis an error term and i corresponds to a specific household. Report the results of the regression in a table. At a minimum, your table should contain the estimated parameters, the standard errors, the t-statistics and the p-values for the standard tests of the hypothesis that the parameters are equal to zero.
Please note: You should construct all of the quantities from scratch using their definition from linear econometrics. The same observation applies to all other questions below. You can use a Python regression function only to check your results.
(4) (3 points) What does the model say about the determinants of (log) medical expenditures? You should comment on the sign, statistical and economic significance of the estimated coefficients.
(5) (3 points) In a regression - without log transformations - of y on x the regression coefficient mea代 写Nonlinear econometrics for finance HOMEWORK 1Python
代做程序编程语言sures ∆y/∆x. What is the interpretation of θ1 here? Hint: you are regressing a log variable (log(medexpi)) on a variable that is not in logs (agei).
(6) (3 points) What is the interpretation of θ4? Hint: you are regressing a log variable (log(medexpi)) on another log variable (log(totalexpi)).
(7) (4 points) We want to test whether the coefficient θ4 for log(totalexp) is statistically significant. Test the hypothesis using the relevant test statistic. Does log(totalexp) have more or less explanatory power than age?
(8) (3 points) We want to test whether the coefficient θ4 for log(totalexp) is statistically significant. Test the hypothesis using the relevant p-value.
(9) (5 points) Test the single linear restriction θ2 = −5θ1 using the relevant test statistic.
(10) (3 points) Test the single linear restriction θ2 = −5θ1 using the relevant p-value.
(11) (5 points) Test the multiple linear restriction θ2 = −0.05 and θ3 = 0.05 using the relevant test statistic.
(12) (3 points) Test the multiple linear restriction θ2 = −0.05 and θ3 = 0.05 using the relevant p-value.
(13) (4 points) Using the estimated model, predict medical costs for a house-hold whose head is 36 years old, has 10 years of education, the house-hold size is 4 and the total logarithm of expenditures is 10. Is the prediction lower or higher than the mean of the distribution of the medical expenses? (Recall that the regression gives you a prediction for the log of the medical costs (say, log(y)) not for the medical costs (say, y). Hence, after you find the prediction for the log of the medical costs, you need to make a transformation to find a prediction for the medical costs themselves. Hint: if log(y) is normal, y is lognormal. What is E(y) for a log normal random variable? )
Now, take the categorical variables (excluding “community”, which you should ignore) into account using dummy variables (https://en.wikipedia.org/wiki/Dummy_variable_(statistics)). Re-run the regression using the cat-egorical variables.
(14) (3 points) Which dummies are statistically significant?
(15) (3 points) How much more (or less) do households with males heads spend relative to households led by female heads (controlling for all other variables)?
(16) (3 points) How much more (or less) do farming households spend rela-tive to non farming households (controlling for all other variables)?
(17) (3 points) Using your model, predict medical expenses for a non-farming, urban household whose head is a 43 years old male with 10 years of education, in which there are 3 people and total expenditure is 45,000.





         
加QQ：99515681  WX：codinghelp
