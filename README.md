# Exploratory Data Analysis and Regression Analysis of P_Content and Year
# Source of DataSet: 
On life satisfaction, children in Ireland rated themselves as having one of the lowest rates in the OECD/EU
(72%), with 28% marking a score of 5 or under on a scale of 10 (UNICEF Office of Research). Among the
issues contributing to these low scores, body image, pressure to succeed in school and bullying.
The Health Behaviour in School-aged Children (HBSC) survey is a WHO collaborative cross-national study
that monitors the health behaviours, health outcomes and social environments of school-aged children every
four years. The HBSC Ireland team, based at the Health Promotion Research Centre, University of Galway
conducted the nationally representative survey of Irish school children in 2006, 2010, 2014 and 2018. This
data set contains:
• P_Content The percentage of children that reported being happy with they way they are,
• Age the Age of the child,
• Sex the Sex of the child Male or Female
• Year the Year the information was collected,
# Objective: 
The objective of this project is to carryout exploratory data analysis on the dataset and fit a simple linear regression model to the data with P_Content as the response variable and Year as a numeric predictor variable for females.
# Summary of Exploratory Data Analysis
- The minimum P_Content for each of the year is slightly different from one another
- The female and the male gender has the same frequency for each of the year. i.e. No of female = No of male = 8 for the year 2006, 2010, 2014, 2018.
# Summary of Regression model
- linearMod <- lm(P_Content ~Year, data = df_female)
- The intercept has a value of 655.0157, which implies that is the value of the P_Content when no year is
involved.
- This model estimates that increasing the Year by an additional year when the information was collectecd it will
result in a -0.2944 decrease of the P_Content.
- The standard error of the regression intercept(699.2138) was large relative to the coefficientestimate(655.0157) of the regression intercept, the predictor variable was not statistically significant.
- The standard error of the regression slope( 0.3475209) was large relative to the coefficientestimate(-0.2944) of the regression slope, the predictor variable was not statistically significant
