# Analysing factors that affect Red Wine Quality

This project is performing Data Analysis on properties on red wine and understanding which parameter influences the quality.

#### File Description
The following files are a part of this project.  
1. wine-preference-modelling-r.Rproj : RStudio project file  
2. project_code.Rmd : R Markdown file containing entire source code  
3. project_code.html : Knitted HTML file  
4. wineQualityReds.csv : Downloaded from the reference below. Not available in the project repository here.  


#### Required R Libraries

The following libraries were used in this project. It is must to install these libraries before running the project.  
1. ggplot2  
2. GGally  
3. Cowplot  

The entire analysis is available in the HTML file. The reflection and references of this project is mentioned below :  

### Reflection

It is time to reflect all the observations. First, we tried to observe how each individual variable varies. We found that quality of red wine follows normal distribution with majority of quality values fall near to the mean. The fixed acidity and volatile acidity also follows normal distribution. The residual sugar value does not seem to follow normal ditribution. Most values fall near the range of 1 to 3 while some outliers extending upto 15. The chlorides have most values less than 0.15. Some values fall in the higher range. It would be interesting to see if any of these outliers have higher quality. The Free Sulfur Dioxide value and Total Sulfur Dioxide value also fall in the lower range. The red wine density seems to follow normal distribution with mean at around 0.9975.  

In the bivariate analysis, we find the correlation of quality with rest other variables. We see that Alcohol content has the highest correlation with quality followed by volatile acidity and sulphates. The correlation values also show that residual sugar and pH should have very less effect on the quality as these correlation values are closer to 0.  

In the multivariate analysis, the plots did not give a very clear idea. But we could see that the alcohol content has positive effect on the quality. To get a clear picture, we binned the quality into four categories (bad, average, good, very good). Most of the values fell into average and good bins. We again ran the plots with these values and found out that alcohol clearly has positive effect on the quality. When alcohol and citric acid both are high, there is higher probability for the red wine to be of good quality. The suphates did not show much variation. They had very less effect on the quality. The volatile acidity clearly showed negative effect on the quality. Lower the volatile acidity, higher would be the quality.  

The further analysis of this project would include comparing every two variables against the quality and find which two variables affect the quality the most. We took alcohol in most of the example as the correlation showed positive influence of alcohol on acidity.

#### References :

The dataset was downloaded from the folowing reference :  



P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. 
  Modeling wine preferences by data mining from physicochemical properties.
  In Decision Support Systems, Elsevier, 47(4):547-553. ISSN: 0167-9236.

  Available at: [@Elsevier] http://dx.doi.org/10.1016/j.dss.2009.05.016  
                [Pre-press (pdf)] http://www3.dsi.uminho.pt/pcortez/winequality09.pdf  
                [bib] http://www3.dsi.uminho.pt/pcortez/dss09.bib  

