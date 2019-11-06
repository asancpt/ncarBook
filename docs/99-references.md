
# R에 내장된 자료의 비구획분석 보고서 {#groupreport}

## Theoph의 보고서 {#theophgroup}


```r
ID=6

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
     0.0000       0.0000                           0.0000     0.0000
     0.2700       1.2900                           0.1742     0.0470
     0.5800       3.0800                           0.8515     0.3779
     1.1500       6.4400                           3.5647     2.9977
     2.0300 *     6.3200     6.3928 -7.284e-02     9.1791    11.9014
     3.5700 *     5.5300     5.5844 -5.438e-02    18.3036    36.9816
     5.0000 *     4.9400     4.9255 +1.450e-02    25.7897    68.7577
     7.0000 *     4.0200     4.1323 -1.123e-01    34.7497   121.5977
     9.2200 *     3.4600     3.4005 +5.948e-02    43.0525   188.2434
    12.1000 *     2.7800     2.6408 +1.392e-01    52.0381   282.6199
    23.8500 *     0.9200     0.9413 -2.127e-02    73.7756   609.1524

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        6.4400 mg/L
CMAXD      Max Conc Norm by Dose                           0.0201 mg/L/mg
TMAX       Time of CMAX                                    1.1500 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               0.9200 mg/L
CLSTP      Last Nonzero Conc Pred                          0.9413 mg/L
TLST       Time of Last Nonzero Conc                      23.8500 h
LAMZHL     Half-Life Lambda z                              7.8950 h
LAMZ       Lambda z                                        0.0878 /h
LAMZLL     Lambda z Lower Limit                            2.0300 h
LAMZUL     Lambda z Upper Limit                           23.8500 h
LAMZNPT    Number of Points for Lambda z                   7
CORRXY     Correlation Between TimeX and Log ConcY        -0.9991 
R2         R Squared                                       0.9982 
R2ADJ      R Squared Adjusted                              0.9979 
AUCLST     AUC to Last Nonzero Conc                       73.7756 h*mg/L
AUCALL     AUC All                                        73.7756 h*mg/L
AUCIFO     AUC Infinity Obs                               84.2544 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.2633 h*mg/L/mg
AUCIFP     AUC Infinity Pred                              84.4967 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.2641 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         12.4372 %
AUCPEP     AUC %Extrapolation Pred                        12.6882 %
AUMCLST    AUMC to Last Nonzero Conc                     609.1524 h2*mg/L
AUMCIFO    AUMC Infinity Obs                             978.4285 h2*mg/L
AUMCIFP    AUMC Infinity Pred                            986.9665 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        37.7418 %
AUMCPEP    AUMC % Extrapolation Pred                      38.2803 %
VZFO       Vz Obs by F                                    43.2597 L
VZFP       Vz Pred by F                                   43.1357 L
CLFO       Total CL Obs by F                               3.7980 L/h
CLFP       Total CL Pred by F                              3.7871 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.2568 h
MRTEVIFO   MRT Extravasc Infinity Obs                     11.6128 h
MRTEVIFP   MRT Extravasc Infinity Pred                    11.6805 h





ID=7

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
     0.0000       0.1500                           0.0000     0.0000
     0.2500       0.8500                           0.1250     0.0266
     0.5000       2.3500                           0.5250     0.2000
     1.0200       5.0200                           2.4412     1.8368
     2.0200       6.5800                           8.2412    11.0428
     3.4800       7.0900                          18.2203    38.7571
     5.0000       6.6600                          28.6703    82.8167
     6.9800 *     5.2500     5.3226 -7.260e-02    40.4612   152.0623
     9.0000 *     4.3900     4.4527 -6.275e-02    50.1976   228.9788
    12.0500 *     3.5300     3.4011 +1.289e-01    62.2756   354.0998
    24.2200 *     1.1500     1.1607 -1.072e-02    90.7534   782.4199

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        7.0900 mg/L
CMAXD      Max Conc Norm by Dose                           0.0222 mg/L/mg
TMAX       Time of CMAX                                    3.4800 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.1500 mg/L
CLSTP      Last Nonzero Conc Pred                          1.1607 mg/L
TLST       Time of Last Nonzero Conc                      24.2200 h
LAMZHL     Half-Life Lambda z                              7.8467 h
LAMZ       Lambda z                                        0.0883 /h
LAMZLL     Lambda z Lower Limit                            6.9800 h
LAMZUL     Lambda z Upper Limit                           24.2200 h
LAMZNPT    Number of Points for Lambda z                   4
CORRXY     Correlation Between TimeX and Log ConcY        -0.9993 
R2         R Squared                                       0.9987 
R2ADJ      R Squared Adjusted                              0.9980 
AUCLST     AUC to Last Nonzero Conc                       90.7534 h*mg/L
AUCALL     AUC All                                        90.7534 h*mg/L
AUCIFO     AUC Infinity Obs                              103.7718 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.3243 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             103.8931 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.3247 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         12.5452 %
AUCPEP     AUC %Extrapolation Pred                        12.6474 %
AUMCLST    AUMC to Last Nonzero Conc                     782.4199 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1245.0984 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1249.4111 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        37.1600 %
AUMCPEP    AUMC % Extrapolation Pred                      37.3769 %
VZFO       Vz Obs by F                                    34.9084 L
VZFP       Vz Pred by F                                   34.8677 L
CLFO       Total CL Obs by F                               3.0837 L/h
CLFP       Total CL Pred by F                              3.0801 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.6214 h
MRTEVIFO   MRT Extravasc Infinity Obs                     11.9984 h
MRTEVIFP   MRT Extravasc Infinity Pred                    12.0259 h





ID=8

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
     0.0000       0.0000                           0.0000     0.0000
     0.2500       3.0500                           0.3813     0.0953
     0.5200       3.0500                           1.2048     0.4124
     0.9800       7.3100                           3.5875     2.4248
     2.0200       7.5600                          11.3200    14.0910
     3.5300 *     6.5900     6.5724 +1.758e-02    22.0032    43.1841
     5.0500 *     5.8800     5.8071 +7.292e-02    31.4804    83.4312
     7.1500 *     4.7300     4.8941 -1.641e-01    42.6209   150.1204
     9.0700 *     4.5700     4.1856 +3.844e-01    51.5489   222.3790
    12.1000 *     3.0000     3.2702 -2.702e-01    63.0175   340.1701
    24.1200 *     1.2500     1.2285 +2.147e-02    88.5600   739.5346

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        7.5600 mg/L
CMAXD      Max Conc Norm by Dose                           0.0236 mg/L/mg
TMAX       Time of CMAX                                    2.0200 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.2500 mg/L
CLSTP      Last Nonzero Conc Pred                          1.2285 mg/L
TLST       Time of Last Nonzero Conc                      24.1200 h
LAMZHL     Half-Life Lambda z                              8.5100 h
LAMZ       Lambda z                                        0.0815 /h
LAMZLL     Lambda z Lower Limit                            3.5300 h
LAMZUL     Lambda z Upper Limit                           24.1200 h
LAMZNPT    Number of Points for Lambda z                   6
CORRXY     Correlation Between TimeX and Log ConcY        -0.9955 
R2         R Squared                                       0.9910 
R2ADJ      R Squared Adjusted                              0.9888 
AUCLST     AUC to Last Nonzero Conc                       88.5600 h*mg/L
AUCALL     AUC All                                        88.5600 h*mg/L
AUCIFO     AUC Infinity Obs                              103.9067 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.3247 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             103.6431 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.3239 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         14.7697 %
AUCPEP     AUC %Extrapolation Pred                        14.5529 %
AUMCLST    AUMC to Last Nonzero Conc                     739.5346 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1298.1158 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1288.5201 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        43.0302 %
AUMCPEP    AUMC % Extrapolation Pred                      42.6059 %
VZFO       Vz Obs by F                                    37.8105 L
VZFP       Vz Pred by F                                   37.9067 L
CLFO       Total CL Obs by F                               3.0797 L/h
CLFP       Total CL Pred by F                              3.0875 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.3507 h
MRTEVIFO   MRT Extravasc Infinity Obs                     12.4931 h
MRTEVIFP   MRT Extravasc Infinity Pred                    12.4323 h





ID=11

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
     0.0000       0.0000                           0.0000     0.0000
     0.2500       4.8600                           0.6075     0.1519
     0.5000       7.2400                           2.1200     0.7563
     0.9800       8.0000                           5.7776     3.5067
     1.9800       6.8100                          13.1826    14.1686
     3.6000       5.8700                          23.4534    42.2073
     5.0200       5.2200                          31.3273    75.8162
     7.0300       4.4500                          41.0457   133.5915
     9.0300 *     3.6200     3.6169 +3.150e-03    49.1156   197.5636
    12.1200 *     2.6900     2.6929 -2.948e-03    58.8646   298.4388
    24.0800 *     0.8600     0.8598 +1.934e-04    80.0936   617.2422

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        8.0000 mg/L
CMAXD      Max Conc Norm by Dose                           0.0250 mg/L/mg
TMAX       Time of CMAX                                    0.9800 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               0.8600 mg/L
CLSTP      Last Nonzero Conc Pred                          0.8598 mg/L
TLST       Time of Last Nonzero Conc                      24.0800 h
LAMZHL     Half-Life Lambda z                              7.2612 h
LAMZ       Lambda z                                        0.0955 /h
LAMZLL     Lambda z Lower Limit                            9.0300 h
LAMZUL     Lambda z Upper Limit                           24.0800 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -1.0000 
R2         R Squared                                       1.0000 
R2ADJ      R Squared Adjusted                              1.0000 
AUCLST     AUC to Last Nonzero Conc                       80.0936 h*mg/L
AUCALL     AUC All                                        80.0936 h*mg/L
AUCIFO     AUC Infinity Obs                               89.1027 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.2784 h*mg/L/mg
AUCIFP     AUC Infinity Pred                              89.1007 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.2784 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         10.1110 %
AUCPEP     AUC %Extrapolation Pred                        10.1089 %
AUMCLST    AUMC to Last Nonzero Conc                     617.2422 h2*mg/L
AUMCIFO    AUMC Infinity Obs                             928.5600 h2*mg/L
AUMCIFP    AUMC Infinity Pred                            928.4900 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        33.5269 %
AUMCPEP    AUMC % Extrapolation Pred                      33.5219 %
VZFO       Vz Obs by F                                    37.6222 L
VZFP       Vz Pred by F                                   37.6230 L
CLFO       Total CL Obs by F                               3.5914 L/h
CLFP       Total CL Pred by F                              3.5914 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              7.7065 h
MRTEVIFO   MRT Extravasc Infinity Obs                     10.4212 h
MRTEVIFP   MRT Extravasc Infinity Pred                    10.4207 h





ID=3

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
     0.0000       0.0000                           0.0000     0.0000
     0.2700       4.4000                           0.5940     0.1604
     0.5800       6.9000                           2.3455     0.9648
     1.0200       8.2000                           5.6675     3.6854
     2.0200       7.8000                          13.6675    15.7453
     3.6200       7.5000                          25.9075    50.0702
     5.0800       6.2000                          35.9085    92.8817
     7.0700       5.3000                          47.3510   161.5039
     9.0000 *     4.9000     4.9914 -9.138e-02    57.1940   240.2199
    12.1500 *     3.7000     3.6147 +8.528e-02    70.7390   380.4815
    24.1700 *     1.0500     1.0551 -5.097e-03    99.2865   803.1859

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        8.2000 mg/L
CMAXD      Max Conc Norm by Dose                           0.0256 mg/L/mg
TMAX       Time of CMAX                                    1.0200 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.0500 mg/L
CLSTP      Last Nonzero Conc Pred                          1.0551 mg/L
TLST       Time of Last Nonzero Conc                      24.1700 h
LAMZHL     Half-Life Lambda z                              6.7661 h
LAMZ       Lambda z                                        0.1024 /h
LAMZLL     Lambda z Lower Limit                            9.0000 h
LAMZUL     Lambda z Upper Limit                           24.1700 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -0.9997 
R2         R Squared                                       0.9993 
R2ADJ      R Squared Adjusted                              0.9986 
AUCLST     AUC to Last Nonzero Conc                       99.2865 h*mg/L
AUCALL     AUC All                                        99.2865 h*mg/L
AUCIFO     AUC Infinity Obs                              109.5360 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.3423 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             109.5857 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.3425 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                          9.3572 %
AUCPEP     AUC %Extrapolation Pred                         9.3983 %
AUMCLST    AUMC to Last Nonzero Conc                     803.1859 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1150.9648 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1152.6529 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        30.2163 %
AUMCPEP    AUMC % Extrapolation Pred                      30.3185 %
VZFO       Vz Obs by F                                    28.5171 L
VZFP       Vz Pred by F                                   28.5042 L
CLFO       Total CL Obs by F                               2.9214 L/h
CLFP       Total CL Pred by F                              2.9201 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.0896 h
MRTEVIFO   MRT Extravasc Infinity Obs                     10.5076 h
MRTEVIFP   MRT Extravasc Infinity Pred                    10.5183 h





ID=2

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
     0.0000       0.0000                           0.0000     0.0000
     0.2700       1.7200                           0.2322     0.0627
     0.5200       7.9100                           1.4360     0.6349
     1.0000       8.3100                           5.3287     3.6165
     1.9200       8.3300                          12.9832    14.7961
     3.5000       6.8500                          24.9754    46.3713
     5.0200       6.0800                          34.8022    87.7887
     7.0300 *     5.4000     5.3629 +3.707e-02    46.3396   156.6147
     9.0000 *     4.5500     4.3687 +1.813e-01    56.1403   234.3431
    12.0000 *     3.0100     3.1970 -1.870e-01    67.4803   349.9481
    24.3000 *     0.9000     0.8886 +1.136e-02    91.5268   706.5866

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        8.3300 mg/L
CMAXD      Max Conc Norm by Dose                           0.0260 mg/L/mg
TMAX       Time of CMAX                                    1.9200 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               0.9000 mg/L
CLSTP      Last Nonzero Conc Pred                          0.8886 mg/L
TLST       Time of Last Nonzero Conc                      24.3000 h
LAMZHL     Half-Life Lambda z                              6.6593 h
LAMZ       Lambda z                                        0.1041 /h
LAMZLL     Lambda z Lower Limit                            7.0300 h
LAMZUL     Lambda z Upper Limit                           24.3000 h
LAMZNPT    Number of Points for Lambda z                   4
CORRXY     Correlation Between TimeX and Log ConcY        -0.9986 
R2         R Squared                                       0.9972 
R2ADJ      R Squared Adjusted                              0.9958 
AUCLST     AUC to Last Nonzero Conc                       91.5268 h*mg/L
AUCALL     AUC All                                        91.5268 h*mg/L
AUCIFO     AUC Infinity Obs                              100.1735 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.3130 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             100.0643 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.3127 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                          8.6317 %
AUCPEP     AUC %Extrapolation Pred                         8.5320 %
AUMCLST    AUMC to Last Nonzero Conc                     706.5866 h2*mg/L
AUMCIFO    AUMC Infinity Obs                             999.7723 h2*mg/L
AUMCIFP    AUMC Infinity Pred                            996.0716 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        29.3252 %
AUMCPEP    AUMC % Extrapolation Pred                      29.0627 %
VZFO       Vz Obs by F                                    30.6904 L
VZFP       Vz Pred by F                                   30.7239 L
CLFO       Total CL Obs by F                               3.1945 L/h
CLFP       Total CL Pred by F                              3.1979 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              7.7200 h
MRTEVIFO   MRT Extravasc Infinity Obs                      9.9804 h
MRTEVIFP   MRT Extravasc Infinity Pred                     9.9543 h





ID=4

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
     0.0000       0.0000                           0.0000     0.0000
     0.3500       1.8900                           0.3308     0.1158
     0.6000       4.6000                           1.1420     0.5435
     1.0700       8.6000                           4.2440     3.3545
     2.1300       8.3800                          13.2434    17.6918
     3.5000       7.5400                          24.1486    47.9958
     5.0200       6.8800                          35.1078    94.3007
     7.0200       5.7800                          47.7678   169.4139
     9.0200 *     5.3300     5.4586 -1.286e-01    58.8778   258.0661
    11.9800 *     4.1900     4.0686 +1.214e-01    72.9674   403.5099
    24.6500 *     1.1500     1.1564 -6.422e-03   106.7963   901.0842

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        8.6000 mg/L
CMAXD      Max Conc Norm by Dose                           0.0269 mg/L/mg
TMAX       Time of CMAX                                    1.0700 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.1500 mg/L
CLSTP      Last Nonzero Conc Pred                          1.1564 mg/L
TLST       Time of Last Nonzero Conc                      24.6500 h
LAMZHL     Half-Life Lambda z                              6.9812 h
LAMZ       Lambda z                                        0.0993 /h
LAMZLL     Lambda z Lower Limit                            9.0200 h
LAMZUL     Lambda z Upper Limit                           24.6500 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -0.9995 
R2         R Squared                                       0.9989 
R2ADJ      R Squared Adjusted                              0.9978 
AUCLST     AUC to Last Nonzero Conc                      106.7963 h*mg/L
AUCALL     AUC All                                       106.7963 h*mg/L
AUCIFO     AUC Infinity Obs                              118.3789 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.3699 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             118.4436 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.3701 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                          9.7843 %
AUCPEP     AUC %Extrapolation Pred                         9.8336 %
AUMCLST    AUMC to Last Nonzero Conc                     901.0842 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1303.2524 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1305.4981 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        30.8588 %
AUMCPEP    AUMC % Extrapolation Pred                      30.9777 %
VZFO       Vz Obs by F                                    27.2260 L
VZFP       Vz Pred by F                                   27.2111 L
CLFO       Total CL Obs by F                               2.7032 L/h
CLFP       Total CL Pred by F                              2.7017 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.4374 h
MRTEVIFO   MRT Extravasc Infinity Obs                     11.0092 h
MRTEVIFP   MRT Extravasc Infinity Pred                    11.0221 h





ID=9

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
     0.0000       0.0000                           0.0000     0.0000
     0.3000       7.3700                           1.1055     0.3316
     0.6300       9.0300                           3.8115     1.6351
     1.0500       7.1400                           7.2072     4.4042
     2.0200       6.3300                          13.7402    14.2417
     3.5300       5.6600                          22.7926    38.9804
     5.0200       5.6700                          31.2335    75.0705
     7.1700       4.2400                          41.8867   138.3495
     8.8000 *     4.1100     4.0512 +5.880e-02    48.6920   192.6031
    11.6000 *     3.1600     3.2160 -5.597e-02    58.8700   294.5567
    24.4300 *     1.1200     1.1165 +3.517e-03    86.3262   705.2296

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        9.0300 mg/L
CMAXD      Max Conc Norm by Dose                           0.0282 mg/L/mg
TMAX       Time of CMAX                                    0.6300 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.1200 mg/L
CLSTP      Last Nonzero Conc Pred                          1.1165 mg/L
TLST       Time of Last Nonzero Conc                      24.4300 h
LAMZHL     Half-Life Lambda z                              8.4060 h
LAMZ       Lambda z                                        0.0825 /h
LAMZLL     Lambda z Lower Limit                            8.8000 h
LAMZUL     Lambda z Upper Limit                           24.4300 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -0.9997 
R2         R Squared                                       0.9994 
R2ADJ      R Squared Adjusted                              0.9989 
AUCLST     AUC to Last Nonzero Conc                       86.3262 h*mg/L
AUCALL     AUC All                                        86.3262 h*mg/L
AUCIFO     AUC Infinity Obs                               99.9087 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.3122 h*mg/L/mg
AUCIFP     AUC Infinity Pred                              99.8661 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.3121 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         13.5950 %
AUCPEP     AUC %Extrapolation Pred                        13.5581 %
AUMCLST    AUMC to Last Nonzero Conc                     705.2296 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1201.7715 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1200.2124 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        41.3175 %
AUMCPEP    AUMC % Extrapolation Pred                      41.2413 %
VZFO       Vz Obs by F                                    38.8428 L
VZFP       Vz Pred by F                                   38.8594 L
CLFO       Total CL Obs by F                               3.2029 L/h
CLFP       Total CL Pred by F                              3.2043 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.1694 h
MRTEVIFO   MRT Extravasc Infinity Obs                     12.0287 h
MRTEVIFP   MRT Extravasc Infinity Pred                    12.0182 h





ID=12

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
     0.0000       0.0000                           0.0000     0.0000
     0.2500       1.2500                           0.1563     0.0391
     0.5000       3.9600                           0.8075     0.3256
     1.0000       7.8200                           3.7525     2.7756
     2.0000       9.7200                          12.5225    16.4056
     3.5200       9.7500                          27.3197    57.2632
     5.0700       8.5700                          41.5177   117.5349
     7.0700       6.5900                          56.6777   207.5761
     9.0300 *     6.1100     6.2267 -1.167e-01    69.1237   307.3054
    12.0500 *     4.5700     4.4632 +1.068e-01    85.2505   473.7705
    24.1500 *     1.1700     1.1755 -5.539e-03   119.9775   977.8807

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                        9.7500 mg/L
CMAXD      Max Conc Norm by Dose                           0.0305 mg/L/mg
TMAX       Time of CMAX                                    3.5200 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.1700 mg/L
CLSTP      Last Nonzero Conc Pred                          1.1755 mg/L
TLST       Time of Last Nonzero Conc                      24.1500 h
LAMZHL     Half-Life Lambda z                              6.2865 h
LAMZ       Lambda z                                        0.1103 /h
LAMZLL     Lambda z Lower Limit                            9.0300 h
LAMZUL     Lambda z Upper Limit                           24.1500 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -0.9997 
R2         R Squared                                       0.9994 
R2ADJ      R Squared Adjusted                              0.9988 
AUCLST     AUC to Last Nonzero Conc                      119.9775 h*mg/L
AUCALL     AUC All                                       119.9775 h*mg/L
AUCIFO     AUC Infinity Obs                              130.5888 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.4081 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             130.6391 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.4082 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                          8.1258 %
AUCPEP     AUC %Extrapolation Pred                         8.1611 %
AUMCLST    AUMC to Last Nonzero Conc                     977.8807 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1330.3840 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1332.0528 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        26.4964 %
AUMCPEP    AUMC % Extrapolation Pred                      26.5884 %
VZFO       Vz Obs by F                                    22.2243 L
VZFP       Vz Pred by F                                   22.2157 L
CLFO       Total CL Obs by F                               2.4504 L/h
CLFP       Total CL Pred by F                              2.4495 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.1505 h
MRTEVIFO   MRT Extravasc Infinity Obs                     10.1876 h
MRTEVIFP   MRT Extravasc Infinity Pred                    10.1964 h





ID=10

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
     0.0000       0.2400                           0.0000     0.0000
     0.3700       2.8900                           0.5790     0.1978
     0.7700       5.2200                           2.2011     1.2156
     1.0200       6.4100                           3.6548     2.5353
     2.0500       7.8300                          10.9884    14.1690
     3.5500      10.2100                          24.5184    53.3917
     5.0500       9.1800                          39.0609   115.3451
     7.0800       8.0200                          56.5189   220.0328
     9.3800 *     7.1400     7.0610 +7.903e-02    73.9529   362.3508
    12.1000 *     5.6800     5.7586 -7.858e-02    91.3881   546.9044
    23.7000 *     2.4200     2.4137 +6.308e-03   138.3681  1278.1800

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                       10.2100 mg/L
CMAXD      Max Conc Norm by Dose                           0.0319 mg/L/mg
TMAX       Time of CMAX                                    3.5500 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               2.4200 mg/L
CLSTP      Last Nonzero Conc Pred                          2.4137 mg/L
TLST       Time of Last Nonzero Conc                      23.7000 h
LAMZHL     Half-Life Lambda z                              9.2469 h
LAMZ       Lambda z                                        0.0750 /h
LAMZLL     Lambda z Lower Limit                            9.3800 h
LAMZUL     Lambda z Upper Limit                           23.7000 h
LAMZNPT    Number of Points for Lambda z                   3
CORRXY     Correlation Between TimeX and Log ConcY        -0.9998 
R2         R Squared                                       0.9995 
R2ADJ      R Squared Adjusted                              0.9990 
AUCLST     AUC to Last Nonzero Conc                      138.3681 h*mg/L
AUCALL     AUC All                                       138.3681 h*mg/L
AUCIFO     AUC Infinity Obs                              170.6521 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.5333 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             170.5679 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.5330 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         18.9180 %
AUCPEP     AUC %Extrapolation Pred                        18.8780 %
AUMCLST    AUMC to Last Nonzero Conc                    1278.1800 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            2473.9934 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           2470.8765 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        48.3354 %
AUMCPEP    AUMC % Extrapolation Pred                      48.2702 %
VZFO       Vz Obs by F                                    25.0155 L
VZFP       Vz Pred by F                                   25.0279 L
CLFO       Total CL Obs by F                               1.8752 L/h
CLFP       Total CL Pred by F                              1.8761 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              9.2375 h
MRTEVIFO   MRT Extravasc Infinity Obs                     14.4973 h
MRTEVIFP   MRT Extravasc Infinity Pred                    14.4862 h





ID=1

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





ID=5

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
     0.0000       0.0000                           0.0000     0.0000
     0.3000       2.0200                           0.3030     0.0909
     0.5200       5.6300                           1.1445     0.4796
     1.0000      11.4000                           5.2317     3.9182
     2.0200       9.3300                          15.8040    19.3440
     3.5000       8.7400                          29.1758    55.9271
     5.0200       7.5600                          41.5638   108.0184
     7.0200 *     7.0900     6.9799 +1.101e-01    56.2138   195.7414
     9.1000 *     5.9000     5.8291 +7.091e-02    69.7234   303.3417
    12.0000 *     4.3700     4.5343 -1.643e-01    84.6149   457.2302
    24.3500 *     1.5700     1.5557 +1.430e-02   121.2944  1017.1143

*: Used for the calculation of Lambda z.


Calculated Values
-----------------
CMAX       Max Conc                                       11.4000 mg/L
CMAXD      Max Conc Norm by Dose                           0.0356 mg/L/mg
TMAX       Time of CMAX                                    1.0000 h
TLAG       Time Until First Nonzero Conc                   0.0000 h
CLST       Last Nonzero Conc                               1.5700 mg/L
CLSTP      Last Nonzero Conc Pred                          1.5557 mg/L
TLST       Time of Last Nonzero Conc                      24.3500 h
LAMZHL     Half-Life Lambda z                              8.0023 h
LAMZ       Lambda z                                        0.0866 /h
LAMZLL     Lambda z Lower Limit                            7.0200 h
LAMZUL     Lambda z Upper Limit                           24.3500 h
LAMZNPT    Number of Points for Lambda z                   4
CORRXY     Correlation Between TimeX and Log ConcY        -0.9993 
R2         R Squared                                       0.9986 
R2ADJ      R Squared Adjusted                              0.9980 
AUCLST     AUC to Last Nonzero Conc                      121.2944 h*mg/L
AUCALL     AUC All                                       121.2944 h*mg/L
AUCIFO     AUC Infinity Obs                              139.4198 h*mg/L
AUCIFOD    AUC Infinity Obs Norm by Dose                   0.4357 h*mg/L/mg
AUCIFP     AUC Infinity Pred                             139.2546 h*mg/L
AUCIFPD    AUC Infinity Pred Norm by Dose                  0.4352 h*mg/L/mg
AUCPEO     AUC %Extrapolation Obs                         13.0006 %
AUCPEP     AUC %Extrapolation Pred                        12.8974 %
AUMCLST    AUMC to Last Nonzero Conc                    1017.1143 h2*mg/L
AUMCIFO    AUMC Infinity Obs                            1667.7216 h2*mg/L
AUMCIFP    AUMC Infinity Pred                           1661.7937 h2*mg/L
AUMCPEO    AUMC %Extrapolation Obs                        39.0117 %
AUMCPEP    AUMC % Extrapolation Pred                      38.7942 %
VZFO       Vz Obs by F                                    26.4980 L
VZFP       Vz Pred by F                                   26.5294 L
CLFO       Total CL Obs by F                               2.2952 L/h
CLFP       Total CL Pred by F                              2.2979 L/h
MRTEVLST   MRT Extravasc to Last Nonzero Conc              8.3855 h
MRTEVIFO   MRT Extravasc Infinity Obs                     11.9619 h
MRTEVIFP   MRT Extravasc Infinity Pred                    11.9335 h
```

# 지원 {#support}

패키지와 관련한 모든 의문은 <shan@acp.kr> / +82-2-3010-4614 으로 연락 주시면 빠르게 도움 드리겠습니다.
혹은 StackOverflow^[https://stackoverflow.com]에 영어로 질문 올려주시고 링크를 보내주시면 더 좋습니다.

# 세션 정보 {#session-info}


```r
devtools::session_info()
```

```
## - Session info ----------------------------------------------------------
##  setting  value                       
##  version  R version 3.6.1 (2019-07-05)
##  os       Windows 10 x64              
##  system   x86_64, mingw32             
##  ui       RTerm                       
##  language (EN)                        
##  collate  Korean_Korea.949            
##  ctype    Korean_Korea.949            
##  tz       Asia/Seoul                  
##  date     2019-11-06                  
## 
## - Packages --------------------------------------------------------------
##  package     * version date       lib source        
##  assertthat    0.2.1   2019-03-21 [1] CRAN (R 3.6.1)
##  backports     1.1.5   2019-10-02 [1] CRAN (R 3.6.1)
##  bookdown      0.14    2019-10-01 [1] CRAN (R 3.6.1)
##  callr         3.3.2   2019-09-22 [1] CRAN (R 3.6.1)
##  cli           1.1.0   2019-03-19 [1] CRAN (R 3.6.1)
##  crayon        1.3.4   2017-09-16 [1] CRAN (R 3.6.1)
##  desc          1.2.0   2018-05-01 [1] CRAN (R 3.6.1)
##  devtools      2.2.1   2019-09-24 [1] CRAN (R 3.6.1)
##  digest        0.6.22  2019-10-21 [1] CRAN (R 3.6.1)
##  ellipsis      0.3.0   2019-09-20 [1] CRAN (R 3.6.1)
##  evaluate      0.14    2019-05-28 [1] CRAN (R 3.6.1)
##  fs            1.3.1   2019-05-06 [1] CRAN (R 3.6.1)
##  glue          1.3.1   2019-03-12 [1] CRAN (R 3.6.1)
##  htmltools     0.4.0   2019-10-04 [1] CRAN (R 3.6.1)
##  knitr         1.25    2019-09-18 [1] CRAN (R 3.6.1)
##  magrittr      1.5     2014-11-22 [1] CRAN (R 3.6.1)
##  memoise       1.1.0   2017-04-21 [1] CRAN (R 3.6.1)
##  pkgbuild      1.0.6   2019-10-09 [1] CRAN (R 3.6.1)
##  pkgload       1.0.2   2018-10-29 [1] CRAN (R 3.6.1)
##  prettyunits   1.0.2   2015-07-13 [1] CRAN (R 3.6.1)
##  processx      3.4.1   2019-07-18 [1] CRAN (R 3.6.1)
##  ps            1.3.0   2018-12-21 [1] CRAN (R 3.6.1)
##  R6            2.4.0   2019-02-14 [1] CRAN (R 3.6.1)
##  Rcpp          1.0.2   2019-07-25 [1] CRAN (R 3.6.1)
##  remotes       2.1.0   2019-06-24 [1] CRAN (R 3.6.1)
##  rlang         0.4.1   2019-10-24 [1] CRAN (R 3.6.1)
##  rmarkdown     1.16    2019-10-01 [1] CRAN (R 3.6.1)
##  rprojroot     1.3-2   2018-01-03 [1] CRAN (R 3.6.1)
##  sessioninfo   1.1.1   2018-11-05 [1] CRAN (R 3.6.1)
##  stringi       1.4.3   2019-03-12 [1] CRAN (R 3.6.0)
##  stringr       1.4.0   2019-02-10 [1] CRAN (R 3.6.1)
##  testthat      2.3.0   2019-11-05 [1] CRAN (R 3.6.1)
##  usethis       1.5.1   2019-07-04 [1] CRAN (R 3.6.1)
##  withr         2.1.2   2018-03-15 [1] CRAN (R 3.6.1)
##  xfun          0.10    2019-10-01 [1] CRAN (R 3.6.1)
## 
## [1] C:/Users/cmc/Rlib
## [2] C:/Program Files/R/R-3.6.1/library
```

# 참고문헌 {-}


