Homework 8: Building your own R package
=======================================

Package Installation
--------------------

We will use the `devtools` package to facilitate package development. `Devtools` and my package can be installed with the following commands, and both could be loaded with `library` command.

``` r
library(devtools)
```

``` r
load_all()
#> Loading test
# devtools::install_github('zhengdong91/test')
library(test)
library(gapminder)
```

Function Testing
----------------

There are four functions in the package, we designed `Quantiles` and `Top20GdpPercap` functions to deal with the gapminder dataset, `Quantiles` return the difference of a numeric variable, and `Top20GdpPercap` return the top 20 GdpPercap countries in a particular year. I also inplemented two functions `fbind` and `freq_out` Jenny shared with us in the classes as a practice.

``` r
a <- factor(c("character", "hits", "your", "eyeballs"))
b <- factor(c("but", "integer", "where it", "counts"))
fbind(a, b)
#> [1] character hits      your      eyeballs  but       integer   where it 
#> [8] counts   
#> Levels: but character counts eyeballs hits integer where it your
```

#### Some useful links:

-   [Write your own R package, Part One](https://stat545-ubc.github.io/packages04_foofactors-package-01.html)
-   [Write your own R package, Part Two](https://stat545-ubc.github.io/packages05_foofactors-package-02.html)
