Class 11: Genomics
================
Nicole Chang

# Q5 Proportion of MXL with G\|G genotype

``` r
mxl <- read.csv('373531-SampleGenotypes-Homo_sapiens_Variation_Sample_rs8067378.csv')
head(mxl)
```

      Sample..Male.Female.Unknown. Genotype..forward.strand. Population.s. Father
    1                  NA19648 (F)                       A|A ALL, AMR, MXL      -
    2                  NA19649 (M)                       G|G ALL, AMR, MXL      -
    3                  NA19651 (F)                       A|A ALL, AMR, MXL      -
    4                  NA19652 (M)                       G|G ALL, AMR, MXL      -
    5                  NA19654 (F)                       G|G ALL, AMR, MXL      -
    6                  NA19655 (M)                       A|G ALL, AMR, MXL      -
      Mother
    1      -
    2      -
    3      -
    4      -
    5      -
    6      -

``` r
View(mxl)
```

How many G\|G genotypes I have

``` r
table(mxl$Genotype..forward.strand.) / nrow(mxl)
```


         A|A      A|G      G|A      G|G 
    0.343750 0.328125 0.187500 0.140625 
