# A Problem Statement for the Abalon Data Set 
## Ananya Jayakumar


### Introduction


This problem statement includes the following:

1.  Domain: Biology
2.  Problem Statement:  Find the age of an abalon from measurements made from it's body
3.  Description of Data Set:  9 attributes, 4177 rows
4.  Proposed Solution:  Linear Regression
5.  Benchmark Model:  Linear Regression
6.  Performance Metrics:  MAE
7.  Citations


### Domain:  
Data comes from an original (non-machine-learning) study: 
"The Population Biology of Abalone (_Haliotis_ species) in Tasmania. I. Blacklip Abalone (_H. rubra_) from the North Coast and Islands of Bass Strait", 
Sea Fisheries Division, Technical Report No. 48 (ISSN 1034-3288) 


### Problem Statement:  
Predicting the age of abalone from physical measurements. The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope -- a boring and time-consuming task. Other measurements, which are easier to obtain, are used to predict the age. Further information, such as weather patterns and location (hence food availability) may be required to solve the problem. 

From the original data examples with missing values were removed (the majority having the predicted value missing), and the ranges of the continuous values have been scaled for use with an ANN (by dividing by 200).


### Description of Data Set:  
----------------------------- 
Sex / nominal / -- / M, F, and I (infant) 
Length / continuous / mm / Longest shell measurement 
Diameter	/ continuous / mm / perpendicular to length 
Height / continuous / mm / with meat in shell 
Whole weight / continuous / grams / whole abalone 
Shucked weight / continuous	/ grams / weight of meat 
Viscera weight / continuous / grams / gut weight (after bleeding) 
Shell weight / continuous / grams / after being dried 
Rings / integer / -- / +1.5 gives the age in years 


### Proposed Solution: 
Linear Regression to predict age which is continuous.


### Benchmark Model: 
We could do some exploratory analysis using decision trees, and see if a regression is giving a better understanding of the strength of a variable than a decision tree can.


### Performance Metrics: 
MAE - when normal


### Citations
https://archive.ics.uci.edu/ml/datasets/abalone





