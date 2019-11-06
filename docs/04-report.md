
---
output: html_document
editor_options: 
  chunk_output_type: console
---

# R을 사용한 비구획분석 보고서 {#ncar}

## 이 장에서는 {#summary-ncar}

보고서를 일정한 형식으로 작성하여 다른 사람/기관과 공유하는 것은 중요합니다. 이를 `ncar` 패키지를 사용하여 좀더 쉽게 할 수 있습니다.
이 패키지를 통해서 약동학 파라이터를 보고서 형식의 text, pdf, rtf 파일로 저장할 수 있습니다.
이에 대해 좀더 자세히 알아보겠습니다.

`ncar`의 `DESCRIPTION` 파일을 보면 다음과 같이 설명하고 있습니다.

> Conduct a noncompartmental analysis with industrial strength.
             Some features are
             1) CDISC SDTM terms
             2) Automatic or manual slope selection
             3) Supporting both 'linear-up linear-down' and 'linear-up log-down' method
             4) Interval(partial) AUCs with 'linear' or 'log' interpolation method
             5) Produce pdf, rtf, text report files.
             * Reference: Gabrielsson J, Weiner D. Pharmacokinetic and Pharmacodynamic Data Analysis - Concepts and Applications. 5th ed. 2016. (ISBN:9198299107).



```r
library(tidyverse)
library(ncar)
```

## txtNCA()

우선 저장될 폴더를 확인하면 다음과 같습니다.


```r
getwd()
```

```
## [1] "C:/Users/cmc/asancpt/book-ncar"
```

저장될 폴더를 변경하고자 한다면 setwd("저장될 경로") 이렇게 설정하면 됩니다.

`txtNCA()` 함수를 사용하여 한 대상자에 대한 plain text 보고서를 작성할 수 있습니다.


```r
txtNCA(Theoph[Theoph$Subject=="1","Time"],
       Theoph[Theoph$Subject=="1","conc"], 
       dose=320, doseUnit="mg", concUnit="mg/L", timeUnit="h")
```

또한, Theoph 자료의 약동학 파라미터 분석 결과는 아래와 같이 텍스트파일로 저장할 수 있습니다.


```r
writeLines(txtNCA(Theoph[Theoph$Subject=="1","Time"],
                  Theoph[Theoph$Subject=="1","conc"], 
                  dose=320, doseUnit="mg", concUnit="mg/L",
                  timeUnit="h"), 
           'Output-ncar/txtNCA-Theoph.txt')
```

저장된 파일 내용은 아래와 같습니다.


```bash
                        NONCOMPARTMENTAL ANALYSIS REPORT
                       Package version 0.4.2 (2019-09-27 KST)
                          R version 3.6.1 (2019-07-05)

Date and Time: 2019-11-06 12:28:24 Asia/Seoul

Calculation Setting
-------------------
Drug Administration: Extravascular
Observation count excluding trailing zero: 11
Dose at time 0: 320 mg
AUC Calculation Method: Linear-up Linear-down
Weighting for lambda z: Uniform (Ordinary Least Square, OLS)
Lambda z selection criterion: Heighest adjusted R-squared value with precision=1e-4


Fitting, AUC, AUMC Result
-------------------------
      Time         Conc.      Pred.   Residual       AUC       AUMC
---------------------------------------------------------------------
     0.0000       0.7400                           0.0000     0.0000
     0.2500       2.8400                           0.4475     0.0888
     0.5700       6.5700                           1.9531     0.8015
     1.1200      10.5000                           6.6474     5.0654
     2.0200       9.6600                          15.7194    19.1383
     3.8200       8.5800                          32.1354    66.1982
     5.1000       8.3600                          42.9769   114.4617
     7.0300       7.4700                          58.2529   206.2815
     9.0500 *     6.8900     6.8912 -1.228e-03    72.7565   322.2988
    12.1200 *     5.9400     5.9387 +1.324e-03    92.4505   528.5219
    24.3700 *     3.2800     3.2801 -1.465e-04   148.9231  1459.0711

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                       10.5000 mg/L
CMAXD      Max Conc Norm by Dose                           0.0328 mg/L/mg
TMAX       Time of CMAX                                    1.1200 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               3.2800 mg/L
CLSTP      Last Nonzero Conc Pred                          3.2801 mg/L
TLST       Time of Last Nonzero Conc                      24.3700 h
LAMZHL     Half-Life Lambda z                             14.3044 h
LAMZ       Lambda z                                        0.0485 /h
LAMZLL     Lambda z Lower Limit                            9.0500 h
LAMZUL     Lambda z Upper Limit                           24.3700 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -1.0000 
R2         R Squared                                       1.0000 
R2ADJ      R Squared Adjusted                              1.0000 
AUCLST     AUC to Last Nonzero Conc                      148.9231 h*mg/L
AUCALL     AUC All                                       148.9231 h*mg/L
AUCIFO     AUC Infinity Obs                              216.6119 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.6769 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             216.6150 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.6769 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         31.2489 %
AUCPEP     AUC %Extrapolation Pred                        31.2499 %
AUMCLST    AUMC to Last Nonzero Conc                    1459.0711 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            4505.5348 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           4505.6709 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        67.6160 %
AUMCPEP    AUMC % Extrapolation Pred                      67.6170 %
VZFO       Vz Obs by F                                    30.4867 L
VZFP       Vz Pred by F                                   30.4863 L
CLFO       Total CL Obs by F                               1.4773 L/h
CLFP       Total CL Pred by F                              1.4773 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              9.7975 h
MRTEVIFO   MRT Extravasc Infinity Obs                     20.8000 h
MRTEVIFP   MRT Extravasc Infinity Pred                    20.8004 h
```

한편 `txtNCA2()`를 다음과 같이 정의하면 여러 대상자에 대한 보고서를 작성 가능합니다.


```r
txtNCA2 <- function(dataset){
  dataset %>% 
    as_tibble() %>% 
    group_by(Subject) %>% 
    summarise(res = c(ID = glue::glue('ID={unique(Subject)}\n\n'),
                     txtNCA(Time, 
                           conc, 
                           dose=320, 
                           doseUnit="mg", 
                           concUnit="mg/L", 
                           timeUnit="h")) %>% paste(collapse = '\n')) %>%
    .$res %>%
    paste(collapse = '\n\n\n\n\n\n')
}
```


```r
txtNCA2(Theoph) %>% writeLines('Output-ncar/txtNCA-group-Theoph.txt')
```

저장된 파일 내용은 Appendix \@ref(theophgroup) 에서 확인 가능합니다.

<!--Indometh의 경우 Appendix \@ref(indomethgroup)-->

## pdfNCA()

pdfNCA()로 pdf로 결과를 볼 수 있습니다. (Figure \@ref(fig:pdfnca-output))


```r
ncar::pdfNCA(fileName="Output-ncar/pdfNCA-Theoph.pdf", Theoph, key="Subject", 
             colTime="Time",  colConc="conc", dose=320, doseUnit="mg", 
             timeUnit="h", concUnit="mg/L")
```

```
## png 
##   2
```


```bash
magick -density 150 Output-ncar/pdfNCA-Theoph.pdf Output-ncar/pdfNCA-Theoph-%02d.png
magick montage Output-ncar/pdfNCA-Theoph-01.png Output-ncar/pdfNCA-Theoph-02.png Output-ncar/montage.png
```

```
## /bin/bash: magick: command not found
## /bin/bash: line 1: magick: command not found
```

<div class="figure">
<img src="Output-ncar/montage.png" alt="pdfNCA() output" width="100%" />
<p class="caption">(\#fig:pdfnca-output)pdfNCA() output</p>
</div>

## rtfNCA()

마이크로소프트 워드에서 편집가능한 rtf파일을 만듭니다.


```r
ncar::rtfNCA(fileName="rtfNCA-Theoph.rtf", Theoph, key="Subject", 
             colTime="Time", colConc="conc", dose=320, doseUnit="mg", 
             timeUnit="h", concUnit="mg/L")
```
