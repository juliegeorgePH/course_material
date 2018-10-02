Precision public health
================
Julian Flowers
02/10/2018

## What is precision public health?

  - A recently coined term first appearing in print in 2014(Dolley 2018)
  - Sparse literature
  - Various definitions but all encompass a set of consistent ideas:
      - Use of *big data* and new tehcnology to improve health
      - Data used to give more precise descriptions of populations and
        individuals
      - Application of new techniques and methods
      - “improving the ability to prevent disease, promote health, and
        reduce health disparities in populations by applying emerging
        methods and technologies for measuring disease, pathogens,
        exposures, behaviors, and susceptibility in populations; and
        developing policies and targeted implementation programs to
        improve health” (Khoury and Galea 2016)
      - “requires robust primary surveillance data, rapid application of
        sophisticated analytics to track the geographical distribution
        of disease, and the capacity to act on such
        information”\[Dowell2016\]
      - “Precision public health is characterized by discovering,
        validating, and optimizing care strategies for
        well-characterized population strata”(Arnett and Claas 2016)

## Current and possible uses

Current literature has identified 4 main use cases for precision public
health:

1.  Disease surveillance and signal detection
2.  Risk prediction
3.  Targeting treatment interventions
4.  Improved disease understanding

![Source:(Dolley 2018)](fpubh-06-00068-t001.jpg)

``` r
pdfs <- list.files(pattern = "pdf")
tables <- readtext(pdfs[1])

head(tables$text) %>%
  str_split(., "\\n") %>% data.frame() %>%
  filter(str_detect(., "table"))
```

These are largely in environmental health and communicable disease
control. The only studies identified by Dolley in non-communicable
disease or broader public health relate to diabetes.

## Precision ph vs precision medicine

There has been some debate about the relationship or otherwise between
precision medicince and precision public health. There are number of
strands:

1.  The 4 Ps of precision medicine (….) should be extended to 5 with the
    addition of P for “population”…
2.  Some argue that the two are unconnected
3.  Some argue that the precision medicine is the antihesis of precision
    medicine and that precision medicine may not improve health and may
    increase inequality, and will divert resources and focus away from
    population health and prevention

## Critiques and controveries

## Implications for health intelligence

In some ways these ideas are nothing new - our users and stakeholders
continually want more granularity and timeliness, more comprehensive
data and insight, and actionable data linked to intervention. We have
initiatives like population segmentation

``` r
summary(cars)
```

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

## Including Plots

You can also embed plots, for example:

![](precision_ph_files/figure-gfm/pressure-1.png)<!-- -->

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.

<div id="refs" class="references">

<div id="ref-Arnett2016">

Arnett, Donna K., and Steven A. Claas. 2016. “Precision medicine,
genomics, and public health.” *Diabetes Care*.
<https://doi.org/10.2337/dc16-1763>.

</div>

<div id="ref-Dolley2018">

Dolley, Shawn. 2018. “Big Data’s Role in Precision Public Health.”
*Frontiers in Public Health*.
<https://doi.org/10.3389/fpubh.2018.00068>.

</div>

<div id="ref-Khoury2016a">

Khoury, Muin J., and Sandro Galea. 2016. “Will Precision Medicine
Improve Population Health?” *JAMA*.
<https://doi.org/10.1001/jama.2016.12260>.

</div>

</div>