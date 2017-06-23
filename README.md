Hello Octocat
-------------

I love Octocat. She's the coolest cat in town.

![error
404](https://dl.dropboxusercontent.com/u/11805474/painblogr/biostats/assignments/octocat.png)
\`\` \#\# Assignment 2

    data("anscombe")
    dim.data.frame(anscombe)

    ## [1] 11  8

    colnames(anscombe)

    ## [1] "x1" "x2" "x3" "x4" "y1" "y2" "y3" "y4"

    head(anscombe)

    ##   x1 x2 x3 x4   y1   y2    y3   y4
    ## 1 10 10 10  8 8.04 9.14  7.46 6.58
    ## 2  8  8  8  8 6.95 8.14  6.77 5.76
    ## 3 13 13 13  8 7.58 8.74 12.74 7.71
    ## 4  9  9  9  8 8.81 8.77  7.11 8.84
    ## 5 11 11 11  8 8.33 9.26  7.81 8.47
    ## 6 14 14 14  8 9.96 8.10  8.84 7.04

    tail(anscombe)

    ##    x1 x2 x3 x4    y1   y2   y3    y4
    ## 6  14 14 14  8  9.96 8.10 8.84  7.04
    ## 7   6  6  6  8  7.24 6.13 6.08  5.25
    ## 8   4  4  4 19  4.26 3.10 5.39 12.50
    ## 9  12 12 12  8 10.84 9.13 8.15  5.56
    ## 10  7  7  7  8  4.82 7.26 6.42  7.91
    ## 11  5  5  5  8  5.68 4.74 5.73  6.89

    summary(anscombe)

    ##        x1             x2             x3             x4    
    ##  Min.   : 4.0   Min.   : 4.0   Min.   : 4.0   Min.   : 8  
    ##  1st Qu.: 6.5   1st Qu.: 6.5   1st Qu.: 6.5   1st Qu.: 8  
    ##  Median : 9.0   Median : 9.0   Median : 9.0   Median : 8  
    ##  Mean   : 9.0   Mean   : 9.0   Mean   : 9.0   Mean   : 9  
    ##  3rd Qu.:11.5   3rd Qu.:11.5   3rd Qu.:11.5   3rd Qu.: 8  
    ##  Max.   :14.0   Max.   :14.0   Max.   :14.0   Max.   :19  
    ##        y1               y2              y3              y4        
    ##  Min.   : 4.260   Min.   :3.100   Min.   : 5.39   Min.   : 5.250  
    ##  1st Qu.: 6.315   1st Qu.:6.695   1st Qu.: 6.25   1st Qu.: 6.170  
    ##  Median : 7.580   Median :8.140   Median : 7.11   Median : 7.040  
    ##  Mean   : 7.501   Mean   :7.501   Mean   : 7.50   Mean   : 7.501  
    ##  3rd Qu.: 8.570   3rd Qu.:8.950   3rd Qu.: 7.98   3rd Qu.: 8.190  
    ##  Max.   :10.840   Max.   :9.260   Max.   :12.74   Max.   :12.500

Assignment 3
------------

    ##    x1 x2 x3 x4    y1   y2    y3    y4
    ## 1  10 10 10  8  8.04 9.14  7.46  6.58
    ## 2   8  8  8  8  6.95 8.14  6.77  5.76
    ## 3  13 13 13  8  7.58 8.74 12.74  7.71
    ## 4   9  9  9  8  8.81 8.77  7.11  8.84
    ## 5  11 11 11  8  8.33 9.26  7.81  8.47
    ## 6  14 14 14  8  9.96 8.10  8.84  7.04
    ## 7   6  6  6  8  7.24 6.13  6.08  5.25
    ## 8   4  4  4 19  4.26 3.10  5.39 12.50
    ## 9  12 12 12  8 10.84 9.13  8.15  5.56
    ## 10  7  7  7  8  4.82 7.26  6.42  7.91
    ## 11  5  5  5  8  5.68 4.74  5.73  6.89

<img src="./figures/xy_plot-1.svg" style="display: block; margin: auto;" />

Assignment 4
------------

    library(readr)
    df <- read_csv("analgesic.csv")

    ## Parsed with column specification:
    ## cols(
    ##   ID = col_integer(),
    ##   Group = col_character(),
    ##   Measurement_1 = col_integer(),
    ##   Measurement_2 = col_integer(),
    ##   Measurement_3 = col_integer()
    ## )

    dim.data.frame(df)

    ## [1] 40  5

    colnames(df)

    ## [1] "ID"            "Group"         "Measurement_1" "Measurement_2"
    ## [5] "Measurement_3"

    head(df)

    ## # A tibble: 6 × 5
    ##      ID     Group Measurement_1 Measurement_2 Measurement_3
    ##   <int>     <chr>         <int>         <int>         <int>
    ## 1     1 Analgesic            26            26            21
    ## 2     2 Analgesic            29            26            23
    ## 3     3 Analgesic            24            28            22
    ## 4     4 Analgesic            25            22            24
    ## 5     5 Analgesic            24            28            23
    ## 6     6 Analgesic            22            23            26

    tail(df)

    ## # A tibble: 6 × 5
    ##      ID   Group Measurement_1 Measurement_2 Measurement_3
    ##   <int>   <chr>         <int>         <int>         <int>
    ## 1    35 Placebo            17            21            15
    ## 2    36 Placebo            19            17            15
    ## 3    37 Placebo            14            19            13
    ## 4    38 Placebo            17            19            13
    ## 5    39 Placebo            11            20            18
    ## 6    40 Placebo            15            18            12

    summary(df)

    ##        ID           Group           Measurement_1   Measurement_2 
    ##  Min.   : 1.00   Length:40          Min.   :10.00   Min.   : 8.0  
    ##  1st Qu.:10.75   Class :character   1st Qu.:17.00   1st Qu.:17.0  
    ##  Median :20.50   Mode  :character   Median :20.00   Median :20.0  
    ##  Mean   :20.50                      Mean   :20.12   Mean   :20.7  
    ##  3rd Qu.:30.25                      3rd Qu.:24.00   3rd Qu.:25.0  
    ##  Max.   :40.00                      Max.   :30.00   Max.   :32.0  
    ##  Measurement_3  
    ##  Min.   :12.00  
    ##  1st Qu.:16.00  
    ##  Median :20.50  
    ##  Mean   :20.52  
    ##  3rd Qu.:24.25  
    ##  Max.   :30.00

    library(tidyr)
    library(dplyr)

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

    library(forcats)

    altered_df <- df  %>%
    # Tidy up df data from wide to long format  
      gather(key = Measurements, 
             value = Results, 
             Measurement_1:Measurement_3) %>%
      # Now set grouping factor
      group_by(Measurements) %>%
      # Summarize the data based on mean value across measurements on each individual  
      summarise( Mean = mean(Results)) %>%
      # Ungroup to remove current grouping to allow for future data analysis 
      ungroup()
      # print out final data frame 
      altered_df

    ## # A tibble: 3 × 2
    ##    Measurements   Mean
    ##           <chr>  <dbl>
    ## 1 Measurement_1 20.125
    ## 2 Measurement_2 20.700
    ## 3 Measurement_3 20.525

Assignment 5
------------

Chicken Weights
---------------

    ## Null Hypothesis
    # H0: The chick weights are not dependent on the type of feed.

    ## Alternative hypothesis
    # H1: The chick weights are dependent on the type of feed.

    # Import data
    library(readr)
    chicken <- read_csv("chick-weights.csv")

    ## Parsed with column specification:
    ## cols(
    ##   weight = col_integer(),
    ##   feed = col_character()
    ## )

    # Plot data: boxplot 
    boxplot(weight~feed, data=chicken)

![](README_files/figure-markdown_strict/chicken%20weights-1.png)

    # Statistical test: One-way ANOVA
    chicktest <- aov(weight~feed, data = chicken)
    summary(chicktest)

    ##             Df Sum Sq Mean Sq F value   Pr(>F)    
    ## feed         5 231129   46226   15.37 5.94e-10 ***
    ## Residuals   65 195556    3009                     
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1

    ## Test statistic
    # The grouping factor has more than three levels.

    # Degree of freedom
    Df= 5

    ## p-value
    #p< 0.05

    ## Outcome of analysis
    # The null hypothesis is rejected therefore the chick weights are dependent on the chick feed. 

The Hot Zone
------------

    ## Null Hypothesis
    # H0: The contaminated water does not cause gastroenteritis.

    ## Alternative hypothesis
    # H1: The contaminated water causes gastroenteritis.

    # Import data
    library(knitr)
    GIT <- read_csv("gastroenteritis.csv")

    ## Parsed with column specification:
    ## cols(
    ##   Consumption = col_character(),
    ##   Outcome = col_character()
    ## )

    # Tidy data using scatterplot
    Graph1 <- xtabs(~Consumption + Outcome, data = GIT)
    Graph1

    ##                     Outcome
    ## Consumption          ill not ill
    ##   < 1 glasses/day     39     121
    ##   > 4 glasses/day    265     146
    ##   1 to 4 glasses/day 265     258

    # Plot barplot
    barplot(Graph1, beside = TRUE, ylab = 'Consumption', xlab = 'Outcome' , main = 'Gastroenteritis', col= c('red','grey','black'))
    legend('top', c('<1 glasses/day', '1 to 4 glasses/day', '>4 glasses/day'), fill = c('red','grey',' black'))

![](README_files/figure-markdown_strict/the%20hot%20zone-1.png)

    # Statistical test:Chi-square test
    z <- chisq.test(Graph1, correct = TRUE)
    z

    ## 
    ##  Pearson's Chi-squared test
    ## 
    ## data:  Graph1
    ## X-squared = 74.925, df = 2, p-value < 2.2e-16

    ## Test statistic
    # Analyse 2 categorical data.
    # To determine whether there is an association between two variables.

    # Degree of freedom
    Df= 2

    ## p-value
    # p< 0.05

    ## Outcome of analysis
    # The null hypothesis is rejected therefore consuming contaminated water cause gastroenteritis.

Nausea
------

    ## Null Hypothesis
    # H0: The 5HT3-receptor blocker treatment does not reduce nausea.

    ## Alternative hypothesis
    # H1: The 5HT3-receptor blocker treatment does reduce nausea.

    # Import data
    library(readr)
    Nausea <- read_csv("nausea.csv")

    ## Parsed with column specification:
    ## cols(
    ##   Patient = col_integer(),
    ##   Nausea_before = col_integer(),
    ##   Nausea_after = col_integer()
    ## )

    # Tidy data: the numeric rating scale is anchored at 0 (no nausea) to 6 (severe nausea and vomiting) for the rate of nausea intensity. Therefore remove row 9 (patient 8).

    # Plot data: Line graph
    plot(Nausea$Nausea_before ~ Nausea$Patient, type = "l", ylim = c(0, 6), xlab = "Patient", ylab = "Nausea_score", main = " Intensity of their nausea before and after receiving a 5HT3-receptor blocker", col = "blue", lwd = 2) 
    lines(Nausea$Nausea_after ~ Nausea$Patient, col = "red", lwd = 2)
    legend("top", c("Nausea_before","Nausea_after"), fill = c("blue", "red"))

![](README_files/figure-markdown_strict/Nausea-1.png)

    # Statistical test
    wilcox.test(Nausea$Nausea_before,Nausea$Nausea_after, paired = TRUE)

    ## Warning in wilcox.test.default(Nausea$Nausea_before, Nausea$Nausea_after, :
    ## cannot compute exact p-value with ties

    ## 
    ##  Wilcoxon signed rank test with continuity correction
    ## 
    ## data:  Nausea$Nausea_before and Nausea$Nausea_after
    ## V = 26, p-value = 0.04983
    ## alternative hypothesis: true location shift is not equal to 0

    ## Test statistic
    # The test analyses two variables that are paired and non-parametric in one population group in order to determine the association between them.

    ## p-value
    # p=0.05

    ## Outcome of analysis
    # The null hypothesis is rejected therefore 5HT3-receptor blocker reduces nausea.

Assignment 6
------------

Housing prices
--------------

    ## Null Hypothesis
    # H0: The housing prices do not depend on the interest rates.

    ## Alternative hypothesis
    # H1: The housing prices do depend on the interest rates.

    # Import data
    library(readr)
    Houses <- read_csv("housing-prices.csv")

    ## Parsed with column specification:
    ## cols(
    ##   interest_rate = col_integer(),
    ##   median_house_price_USD = col_integer()
    ## )

    # Tidy data
    Interest = Houses$interest_rate
    House_price= Houses$median_house_price_USD
    head(cbind(Interest,House_price))

    ##      Interest House_price
    ## [1,]       10      183800
    ## [2,]       10      183200
    ## [3,]       10      174900
    ## [4,]        9      173500
    ## [5,]        8      172900
    ## [6,]        7      173200

    # Plot
    plot(Interest,House_price, xlab = "interest_rate", ylab = "median_house_price_USD")
    abline (lm(Houses$median_house_price_USD ~ Houses$interest_rate, data = Houses), col="red", lwd=2)

![](README_files/figure-markdown_strict/Housing%20prices-1.png)

    # Statistical test:Pearson Linear Regression
    # Linear regression
    House1 <- lm(Houses$median_house_price_USD ~ Houses$interest_rate, data = Houses)
    summary(House1)

    ## 
    ## Call:
    ## lm(formula = Houses$median_house_price_USD ~ Houses$interest_rate, 
    ##     data = Houses)
    ## 
    ## Residuals:
    ##    Min     1Q Median     3Q    Max 
    ## -55865 -31631 -16406  27212  80735 
    ## 
    ## Coefficients:
    ##                      Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)            399229      74427   5.364 9.99e-05 ***
    ## Houses$interest_rate   -24309       9205  -2.641   0.0194 *  
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 43180 on 14 degrees of freedom
    ##   (1 observation deleted due to missingness)
    ## Multiple R-squared:  0.3325, Adjusted R-squared:  0.2848 
    ## F-statistic: 6.974 on 1 and 14 DF,  p-value: 0.01937

    # Diagnostic test 1:Homoskedasticity
    plot(x=House1$fitted.values, y=House1$residuals, main = "Homoskedasticity", col="green", lwd=2)
    abline(h=0, col="red", lwd=2)

![](README_files/figure-markdown_strict/Housing%20prices-2.png)

    # Diagnostic test 2: QQ plot
    qqnorm(House1$residuals)
    qqline(House1$residuals)

![](README_files/figure-markdown_strict/Housing%20prices-3.png)

    # Binary outcome variable
    glm(Houses$median_house_price_USD ~ Houses$interest_rate, data = Houses)

    ## 
    ## Call:  glm(formula = Houses$median_house_price_USD ~ Houses$interest_rate, 
    ##     data = Houses)
    ## 
    ## Coefficients:
    ##          (Intercept)  Houses$interest_rate  
    ##               399229                -24309  
    ## 
    ## Degrees of Freedom: 15 Total (i.e. Null);  14 Residual
    ##   (1 observation deleted due to missingness)
    ## Null Deviance:       3.91e+10 
    ## Residual Deviance: 2.61e+10  AIC: 390.8

    ## Test statistic
    # I plotted a scatter plot to check for linear relationship and outliers.
    # The linear diagnostic tests were used to detremine whether: there was a linear trend, the residuals were normally distributed and the residuals have the same variance for all fitted values of y.

    # Degree of freedom
    Df= 15

    ## p-value
    # p< 0.02

    ## Outcome of analysis
    # The null hypothesis is rejected therefore housing prices are dependent on the interest rate.
