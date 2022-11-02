Midterm_review
================
Yinghui Wang
2022-11-02

# Data Type in R

## List

### Create a list

``` r
# use list() function to create a list

list <- list(c(2:11), 5, 
             c("end","is","near"), "end", 
             matrix(data = c(1:12), ncol = 5, nrow = 3, byrow = T),
             list(1,2,3))
```

    ## Warning in matrix(data = c(1:12), ncol = 5, nrow = 3, byrow = T): data length
    ## [12] is not a sub-multiple or multiple of the number of columns [5]

``` r
list
```

    ## [[1]]
    ##  [1]  2  3  4  5  6  7  8  9 10 11
    ## 
    ## [[2]]
    ## [1] 5
    ## 
    ## [[3]]
    ## [1] "end"  "is"   "near"
    ## 
    ## [[4]]
    ## [1] "end"
    ## 
    ## [[5]]
    ##      [,1] [,2] [,3] [,4] [,5]
    ## [1,]    1    2    3    4    5
    ## [2,]    6    7    8    9   10
    ## [3,]   11   12    1    2    3
    ## 
    ## [[6]]
    ## [[6]][[1]]
    ## [1] 1
    ## 
    ## [[6]][[2]]
    ## [1] 2
    ## 
    ## [[6]][[3]]
    ## [1] 3

# Get elements form the list using index

``` r
# get 2 from member 1, 5, 6

list[[1]][1]
```

    ## [1] 2

``` r
list[[5]][1,2]
```

    ## [1] 2

``` r
list[[6]][[2]][1]
```

    ## [1] 2
