Empirical CDF
========================================================

http://chemicalstatistician.wordpress.com/2013/06/24/exploratory-data-analysis-conceptual-foundations-of-empirical-cumulative-distribution-functions/

Empirical Distribution Function

Eric Cai


```r
set.seed(1)
normal.numbers <- rnorm(100)
```


empirical normal cdf

```r
normal.ecdf <- ecdf(normal.numbers)
```



```r
plot(normal.ecdf, xlab = "Quantiles of Random Standard Normal Numbers", ylab = "", 
    main = "Empirical Cumluative Distribution\nStandard Normal Quantiles")
# Add label to y-axis with mtext() side=2 denotes left vertical axis
# line=2.5 sets the position of the label
mtext(text = expression(hat(F)[n](x)), side = 2, line = 2.5)
```

![plot of chunk plot-ecdf](figure/plot-ecdf.png) 


