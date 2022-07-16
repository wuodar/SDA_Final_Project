## Dataset Relevant Information Paragraph
Predicting the age of abalone from physical measurements.  The age of
abalone is determined by cutting the shell through the cone, staining it,
and counting the number of rings through a microscope -- a boring and
time-consuming task.  Other measurements, which are easier to obtain, are
used to predict the age.  Further information, such as weather patterns
and location (hence food availability) may be required to solve the problem.

From the original data examples with missing values were removed (the
majority having the predicted value missing), and the ranges of the
continuous values have been scaled for use with an ANN (by dividing by 200).

Data comes from an original (non-machine-learning) study:

```latex
Warwick J Nash, Tracy L Sellers, Simon R Talbot, Andrew J Cawthorn and
Wes B Ford (1994) "The Population Biology of Abalone (_Haliotis_
species) in Tasmania. I. Blacklip Abalone (_H. rubra_) from the North
Coast and Islands of Bass Strait", Sea Fisheries Division, Technical
Report No. 48 (ISSN 1034-3288)
```

## Features
|Name		    |Data Type	|Meas.	|Description
|---------------|-----------|-------|-----------
|Sex		    |nominal	|		|M, F, and I (infant)
|Length		    |continuous	|mm	    |Longest shell measurement
|Diameter	    |continuous	|mm	    |perpendicular to length
|Height		    |continuous	|mm	    |with meat in shell
|Whole weight	|continuous	|grams	|whole abalone
|Shucked weight	|continuous	|grams	|weight of meat
|Viscera weight	|continuous	|grams	|gut weight (after bleeding)
|Shell weight	|continuous	|grams	|after being dried
|Rings		    |integer	|		|+1.5 gives the age in years

## Task description
The task is to predict the abalone age in years. From the features table you can read that the age is calculated as the value of the `Ring` feature + 1.5. You should start with playing with the data, so do some exploratory data analysis, data cleaning, data preprocessing. Remember about creating plots, it's crucial to create good visualisations of the data that you're working on! Based on that create some model that will try to predict the abalone age. Try different architectures, and select the best one. Also, propose appropriate evaluation metric depends on what approach will you choose (e.g. classification, linear regression). After that, try to adjust the hyperparameters so that the model does its best. After the job is done, please remember to clean your code! Do some refactor, split code into separate files, write appropriate README that sums up your work and explains it to someone who has no idea what's the task is about - it really matters, as this project will act as your portfolio when you start looking for a job!
