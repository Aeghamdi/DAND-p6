---
title: "Explore and Summarize Data"
author: "Abdulelah Alghamdi"
date: "January 18, 2019"
output: 
 html_document:
    fig_caption: yes
    keep_md: yes
    theme: readable
    toc: yes
    
---
##The chosen data set

White Wine Quality.  





# Univariate Plots Section




```
##  [1] "fixed.acidity"        "volatile.acidity"     "citric.acid"         
##  [4] "residual.sugar"       "chlorides"            "free.sulfur.dioxide" 
##  [7] "total.sulfur.dioxide" "density"              "pH"                  
## [10] "sulphates"            "alcohol"              "quality"
```

```
## Observations: 4,898
## Variables: 12
## $ fixed.acidity        <dbl> 7.0, 6.3, 8.1, 7.2, 7.2, 8.1, 6.2, 7.0, 6...
## $ volatile.acidity     <dbl> 0.27, 0.30, 0.28, 0.23, 0.23, 0.28, 0.32,...
## $ citric.acid          <dbl> 0.36, 0.34, 0.40, 0.32, 0.32, 0.40, 0.16,...
## $ residual.sugar       <dbl> 20.70, 1.60, 6.90, 8.50, 8.50, 6.90, 7.00...
## $ chlorides            <dbl> 0.045, 0.049, 0.050, 0.058, 0.058, 0.050,...
## $ free.sulfur.dioxide  <dbl> 45, 14, 30, 47, 47, 30, 30, 45, 14, 28, 1...
## $ total.sulfur.dioxide <dbl> 170, 132, 97, 186, 186, 97, 136, 170, 132...
## $ density              <dbl> 1.0010, 0.9940, 0.9951, 0.9956, 0.9956, 0...
## $ pH                   <dbl> 3.00, 3.30, 3.26, 3.19, 3.19, 3.26, 3.18,...
## $ sulphates            <dbl> 0.45, 0.49, 0.44, 0.40, 0.40, 0.44, 0.47,...
## $ alcohol              <dbl> 8.8, 9.5, 10.1, 9.9, 9.9, 10.1, 9.6, 8.8,...
## $ quality              <ord> 6, 6, 6, 6, 6, 6, 6, 6, 6, 6, 5, 5, 5, 7,...
```

All variables are numerical except for the quality which is represented as a ordered factor.

## Quality


```
##    3    4    5    6    7    8    9 
##   20  163 1457 2198  880  175    5
```

![](2nd_files/figure-html/quality-1.png)<!-- -->

The Quality is normally distributed.  
The minimum is 3 and the maximum is 9. 

We will create new variable to represents the Quality level.  
I will call it quality_level. with the levels given below.

* 0 - 4 : low
* 5 - 6 : good
* 7 - 10 : perfect


```
##     low    good perfect 
##     183    3655    1060
```

![](2nd_files/figure-html/quality_level-1.png)<!-- -->


## Fixed Acidity


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##   3.800   6.300   6.800   6.855   7.300  14.200
```

![](2nd_files/figure-html/fixed_Acidity-1.png)<!-- -->

The Fixed Acidity is normaly distributed.  
The max is 14.2 $g/dm^3$. and the min is 3.8 $g/dm^3$ and median is 6.8 $g/dm^3$.
There are some outliers.

## Volatile acidity


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##  0.0800  0.2100  0.2600  0.2782  0.3200  1.1000
```

![](2nd_files/figure-html/Volatile_Acidity-1.png)<!-- -->

The Volatile Acidity is normaly distributed.  
The max is 1.1 $g/dm^3$ and the min is 0.08 $g/dm^3$ and median is 0.026 $g/dm^3$  
There are some outliers.

## Citric acid


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##  0.0000  0.2700  0.3200  0.3342  0.3900  1.6600
```

![](2nd_files/figure-html/Citric_Acid-1.png)<!-- -->

The Citric Acidity is normaly distributed.  
The max is 1.66 and the min is 0 $g/dm^3$ and median is 0.32 $g/dm^3$.   
There are some outliers.

## Residual sugar


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##   0.600   1.700   5.200   6.391   9.900  65.800
```

![](2nd_files/figure-html/Residual_Sugar-1.png)<!-- -->

The Residual sugar is right skewed distributed.  
The max is 65.8 and the min is 0.6 $g/dm^3$ and median is 5.2 $g/dm^3$.   
There are some outliers.

## Chlorides


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
## 0.00900 0.03600 0.04300 0.04577 0.05000 0.34600
```

![](2nd_files/figure-html/Chlorides-1.png)<!-- -->

The max is 0.346 $g/dm^3$ and the min is 0.009 $g/dm^3$ and median is 0.043 $g/dm^3$.  
There are some outliers.

## Free sulfur dioxide


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##    2.00   23.00   34.00   35.31   46.00  289.00
```

![](2nd_files/figure-html/Free_Sulfur_Dioxide-1.png)<!-- -->

The Free sulfur dioxide is normally distributed.  
The max is 289 $mg/dm^3$ and the min is 2 $mg/dm^3$ and median is 34 $mg/dm^3$.  
There are some outliers.

## Total sulfur dioxide


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##     9.0   108.0   134.0   138.4   167.0   440.0
```

![](2nd_files/figure-html/total_sulfur_dioxide-1.png)<!-- -->

The Total sulfur dioxide is normally distributed.  
The max is 440 $mg/dm^3$ and the min is 9 $mg/dm^3$ and median is 134 $mg/dm^3$.    
There are some outliers.

## Density


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##  0.9871  0.9917  0.9937  0.9940  0.9961  1.0390
```

![](2nd_files/figure-html/Density-1.png)<!-- -->

The Density is normally distributed.  
The max is 1.039 $mg/cm^3$ and the min is 0.9871 $mg/cm^3$ and median is 0.9937 $mg/cm^3$     
There are some outliers.

## pH


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##   2.720   3.090   3.180   3.188   3.280   3.820
```

![](2nd_files/figure-html/PH-1.png)<!-- -->

The pH is normally distributed.  
The max is 3.82 and the min is 2.72 and median is 3.18     
There are some outliers.


## Sulphates


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##  0.2200  0.4100  0.4700  0.4898  0.5500  1.0800
```

![](2nd_files/figure-html/Sulphates-1.png)<!-- -->

The Sulphates is normally distributed.  
The max is 1.08 $g/dm^3$ and the min is 0.22 $g/dm^3$ and median is 0.47 $g/dm^3$.  
There are some outliers.

## Alcohol


```
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##    8.00    9.50   10.40   10.51   11.40   14.20
```

![](2nd_files/figure-html/Alcohol-1.png)<!-- -->

The max is 14.2% and the min is 8% and median is 10.4%.    
There are some outliers.

# Univariate Analysis


### What is the structure of your dataset?

The dataset is about the White Wine and it has 12 variables and 4,898 observations.

### What is/are the main feature(s) of interest in your dataset?

It can not be anything but the Quality.   
That's why we have to figure out what can affect the quality in a positive or a negative way.

### What other features in the dataset do you think will help support your investigation into your feature(s) of interest?

The number of variables is 12 which is not a small number so investigating it will lead to a really surprising and lots of insights in my opinion.  

### Did you create any new variables from existing variables in the dataset?

yes, I created 1 variable it's called "Quality Level" is used to describe the quality rate ( low, good, perfect).  

### Of the features you investigated, were there any unusual distributions? Did you perform any operations on the data to tidy, adjust, or change the form of the data? If so, why did you do this?

There were no unusual distributions.  
just some outliers which i think its better to keep it, because it will be useful for the data to be realistc that will lead the analysis of the relationships between the variables to be more accurate, that's why I will not remove these outliers.  
No missing values and no need to adjust the data.  


# Bivariate Plots Section


##correlation matrix

In order to start the Bivariate section we will begin with the followig correlation matrix plot to visualize the relationship between the variables:

![](2nd_files/figure-html/Correlation_Matrix-1.png)<!-- -->

Since we will mainly focus on the Quality and its relationship with the rest of the variables, we will visualize each variable with the quality in the below plots.  

## Fixed Acidity vs. Quality

![](2nd_files/figure-html/Fixed_Acidity_vs_Quality11-1.png)<!-- -->

It has a small negative effect on the white wine quality.  


## Volatile Acidity vs. Quality

![](2nd_files/figure-html/Volatile_Acidity_vs_Quality11-1.png)<!-- -->

We have to consider the Volatile Acidity as a negative factor to the white wine quality.  
The relationship between them is an Inverse relationship.

## Citric Acid vs. Quality


![](2nd_files/figure-html/Citric_Acid_vs_Quality11-1.png)<!-- -->

If you focus on the line it shows that there is no relationship between the quality and citric acid at all.  


## Residual sugar vs. Quality


![](2nd_files/figure-html/Residual_sugar_vs_Quality11-1.png)<!-- -->

The Residual sugar is effecting the white wine quality in a negative way but not major affect so will look for other variables with stronger affect.


## Chlorides vs. Quality


![](2nd_files/figure-html/chlorides_vs_Quality11-1.png)<!-- -->

Chlorides is effecting the with wine quality in a negative way even though the range of the used amount of Chlorides is too small, the max is 0.346 and min is 0.009.  

## Free sulfur dioxide vs. Quality


![](2nd_files/figure-html/Free_sulfur_dioxide_vs_Quality11-1.png)<!-- -->

No relationship with the white wine quality at all.


## Total sulfur dioxide vs. Quality


![](2nd_files/figure-html/Total_sulfur_dioxide_vs_Quality11-1.png)<!-- -->

Total sulfur dioxide is affecting the quality in a negative way as it's shown in the plot above.


## Density vs. Quality


![](2nd_files/figure-html/Density_vs_Quality11-1.png)<!-- -->

Obviously, it is an inverse relationship, the density reaches the lowest point with the perfect white wine quality.


## PH vs. Quality


![](2nd_files/figure-html/PH_vs_Quality11-1.png)<!-- -->

Positive relationship, the More you use the PH, the more white wine quality you get.


## Sulphates vs. Quality


![](2nd_files/figure-html/Sulphates_vs_Quality11-1.png)<!-- -->

The plot shows clearly that the sulphates is having a positive relationship with the white wine quality but not a strong one.


## Alcohol vs. Quality


![](2nd_files/figure-html/alcohol_vs_Quality11-1.png)<!-- -->

Its very obvious that alcohol variable is playing a big role in the white wine quality.  
Alcohol had strongest Positive relationship with the quality in the hole dataset.


# Bivariate Analysis

#### Talk about some of the relationships you observed in this part of the investigation. How did the feature(s) of interest vary with other features in the dataset?

I investigated and visulized in this part above in order to know the affect of all the variables of the dataset on the quality of the white wine, in order to choose the most important variables that will be focused on to complete this project.  

Variables with Positive relationships are: PH, Sulphates and Alcohol.  
Variables with inversal relationships are: Fixed Acidity, Volatile Acidity, Residual sugar, Chlorides and Total sulfur dioxide.  

#### Did you observe any interesting relationships between the other features (not the main feature(s) of interest)?

I did not excpect that the inversal relationships will be more than the positive relationships, but it was the opposite.  

I can say now that not all variables of any dataset should affect (positivly or negativly) on a particural variable in the same dataset.  

#### What was the strongest relationship you found?

Clearly its the alcohol with the white wine quality.


# Multivariate Plots Section

After the past section we have some ideas about the most affecting variables that we will continue our project investigating it.  

##PH vs Quality
![](2nd_files/figure-html/PH_QUALITY-1.png)<!-- -->


##Alcohol vs Quality


![](2nd_files/figure-html/ALCOHOL_QUALITY-1.png)<!-- -->

##Total sulfur dioxide vs Quality


![](2nd_files/figure-html/Total_sulfur_dioxide_QUALITY-1.png)<!-- -->


##Density vs Quality


![](2nd_files/figure-html/Density_QUALITY-1.png)<!-- -->

##Volatile Acidity vs Quality

![](2nd_files/figure-html/Volatile_Acidity_QUALITY-1.png)<!-- -->

##volatile Acidity vs Alcohol based on Quality Level

We know that alcohol is affecting positively and Volatile acidity is affecting negatively so we will involve both of it based on the quality level in the below plot:

![](2nd_files/figure-html/vars-1.png)<!-- -->

The majority of the low quality white wine(colored in broun) are having small amount of alcohol and having large amount of volatile Acidity.That why most of those points are gathering in the left-top corner.  
while the majority of the pefect quality white wine(colored in green) are having large amount of alcohol and having small amount of volatile Acidity. That why most of those points are gathering in the right-bottom corner.  

# Multivariate Analysis


### Talk about some of the relationships you observed in this part of the investigation. Were there features that strengthened each other in terms of looking at your feature(s) of interest?

We visualized the strongest variables in the dataset and used multi variables plots.  
We made sure that the alcohol effecting the white wine quality positively while th volatile acidity and Total sulfur dioxide are affecting the white wine quality negativly.

### Were there any interesting or surprising interactions between features?

No 

### OPTIONAL: Did you create any models with your dataset? Discuss the strengths and limitations of your model.

No

### Were there any interesting or surprising interactions between features?


### OPTIONAL: Did you create any models with your dataset? Discuss the 
No

# Final Plots and Summary



### Plot One


![](2nd_files/figure-html/finalquality-1.png)<!-- -->

### Description One

The above plot represents the nature and distribution of the most important variable in our dataset which is the quality.  
This helped us to create the new variable ( Quality Level) and helped us to build our plan to invistigate and analys the variables that can play major role in increasing the quality of the white wine and how it can be obtained.

### Plot Two


![](2nd_files/figure-html/alcohol_vs_Qualityfinal-1.png)<!-- -->

### Description Two

The above plot is one of the main keys in our analysis process because it represents the strongest relationship between the quality and the other variables in our data set.  

While i dont have any idea about the wine and i never tried it, this plot have given me an important insight which is the quality of the white wine is mostly related to the amount of alcohol, this can help me if i wanted to bring a bottle of wine to a friend as gift or trying to order it in some restaurant in the future.


### Plot Three

![](2nd_files/figure-html/varsfinal-1.png)<!-- -->

### Description Three

Really useful and clear insights can be taken from this plot.  

It contains one positive variable(alcohol) and another negative variable(volatile acidity) and shows you how thes variables can affect the quality level which is involved too by being represented as the colors  of the plot's shapes.  

The majority of the low quality white wine(colored in broun) are having small amount of alcohol and having large amount of volatile Acidity.That why most of those points are gathering in the left-top corner.  

while the majority of the pefect quality white wine(colored in green) are having large amount of alcohol and having small amount of volatile Acidity. That why most of those points are gathering in the right-bottom corner. 


------

# Reflection

The chosen data set(White Wine Quality) is suitable to perform analysis on the quality of the wine and how to maintain it, the data set contains most of the components that being used in the white wine.  

I am quite surprised because the used amount of the water was not exist in the data set.  

Maybe its related to the density so the more water you use, the less density you get, not quite sure but i think if the water amount was there it will be perfect data set and the analysis would be more useful even for wine manifactoring purposes.  

The dataset contains 4,898 observations with 12 variables.  

I started by exploring each variable individually and looking at the distribution of each one along with a simple comment/insight below the plot.  

There are 11 chemical variables for each observation in the wine dataset which outputs a quality number.  

I used the quality variable to create a categorical factor(new variable) called Quality Level, it devides the quality to three levels low, good and perfect.  

Most important insights is that white wine quality was highly and positively correlated with alcohol.  

Secondly, white wine quality depends on volatile acidity and Total sulfur dioxide but negatively, which means using high levels of volatile acidity or Total sulfur dioxide can lead your wine quality to be low.  

I found this project very important maybe the hardest project in the DAND course so far, it requires knowledge of the R syntax and plot types and plot parameters and which data to use in the same plot and how to visulize it in a proper way to help figuring the insights easly.

#References 

https://ggplot2.tidyverse.org/reference/geom_histogram.html

https://www.rdocumentation.org/packages/tibble/versions/1.4.2/topics/rownames

https://stackoverflow.com/questions/46128392/warning-when-building-a-function-in-r

https://ggplot2.tidyverse.org/reference/geom_bar.html

https://stackoverflow.com/questions/38839923/r-ggplot-bar-plot-with-month-on-x-axis

https://ggplot2.tidyverse.org/reference/

https://www.r-bloggers.com/how-to-expand-color-palette-with-ggplot-and-rcolorbrewer/

https://stackoverflow.com/questions/10438752/adding-x-and-y-axis-labels-in-ggplot2

https://www.nceas.ucsb.edu/~frazier/RSpatialGuides/colorPaletteCheatsheet.pdf

https://ggplot2.tidyverse.org/reference/geom_smooth.html

https://cran.r-project.org/web/packages/corrplot/vignettes/corrplot-intro.html

https://ggplot2.tidyverse.org/reference/ggtheme.html

http://ggplot.yhathq.com/docs/scale_color_brewer.html

https://ggplot2.tidyverse.org/reference/geom_point.html

https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf



