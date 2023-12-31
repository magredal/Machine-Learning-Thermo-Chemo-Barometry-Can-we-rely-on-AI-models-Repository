Hello and welcome!

This is the series of codes used to calibrate and test the different results from the clinopyroxene Thermo-chemo-barometers presented in Agreda-Lopez et al (2023) submitted to Computers and Geosciences journal.

The general workflow goes like this:

1. you will find two folders.  Select the one that you need:

1a. P-T: contains the scripts for estimating pressure (P) and temperature (T).
1b. X: contains the scripts for estimating the liquid composition (X) in equilibrium with clinopyroxene composition.


2. Inside those folders you will find:

2.a An excel file called 'cpx_dat_MAL_pt' that contains the experimental clinopyroxene compositions, pressure and temperatures compiled by Jorgenson et al (2022). This file is used to filter and train the algorithm.
2.b Seven python scripts:
   0-Pre-processing-cpx: Filters the experimental clinopyroxen database.
   1-Model-training: Trains 500 models for P/T/X.
   2-Apply-models-TEST: Applies the trained models to a test data set.
   3-bias-estimation: Calculates the residual of the expected vs. predicted estimates.
   4-bias-correction-models: Creates the five different bias correction models cited in the manuscript.
   5a-Stats-Plots-Results: Calculates the statistics of the estimates with the bias corrections in the test data set and gives the plots presented in the manuscript.
   5b-Stats-Plots-Validation: Calculates the statistics of the estimates with the bias corrections in the validation data set and gives the plots presented in the manuscript.

You will need to run one by one sequentially followinng the order listed above. 

NOTE: the training and bias estimation of this model will take several hours and space in your disk!



If you have any issues please write to: maurizio.petrelli@unipg.it, monica.agredalopez@studenti.unipg.it