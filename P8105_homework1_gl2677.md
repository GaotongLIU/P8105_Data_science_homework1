P8105\_homework1\_gl2677
================
Gaotong LIU (gl2677)
2019-09-20

# Problem 1

## Section 1

Here is a **code chunk** that creates the data frame comprised of:

  - A random sample of size 8 from a standard Normal distribution
  - A logical vector indicating whether elements of the sample are
    greater than 0
  - A character vector of length 8
  - A factor vector of length 8, with 3 different factor
    “levels”

<!-- end list -->

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────────────────────────── tidyverse 1.2.1 ──

    ## ✔ ggplot2 3.2.1     ✔ purrr   0.3.2
    ## ✔ tibble  2.1.3     ✔ dplyr   0.8.3
    ## ✔ tidyr   0.8.3     ✔ stringr 1.4.0
    ## ✔ readr   1.3.1     ✔ forcats 0.4.0

    ## ── Conflicts ────────────────────────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

``` r
sample = rnorm(8)
df = tibble(
  vec_numeric = sample,
  vec_logical = sample > 0,
  vec_char = c("My","name","is","Gaotong","LIU","MS","Biostatistic","T & M"),
  vec_factor = factor(c("High","Low","Medium","High","High","Low","Medium","Low"))
  )
```

I try to take the mean of the variables:

The mean of `vec_numeric` is -0.1740351.

The mean of `vec_logical` is 0.5.

The mean of `vec_char` is NA.

The mean of `vec_factor` is NA.

Therefore, only numeric and logical variables work for `mean()` \#\#
Section 2
