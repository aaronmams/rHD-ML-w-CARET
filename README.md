This repository provides some sample data and code to illustrate a few
of the more interesting features of the
[CARET](https://topepo.github.io/caret/) package for training Machine
Learning models in R.

I have a long-from write-up on the CARET package on [my research
blog](https://aaronmams.github.io/ML-pipelines-in-R-using-caret/).

Code
----

The workhorse of this repository is a .rmd file called
[caret-example.Rmd]()

Dependencies
------------

I have a simulated data set that goes along with this example. The data
set is based on the real structure of Vessel Monitoring System data that
I work with in my professional life. The data file [is here:
fishing\_data.csv]()

It is a .csv file containing ~200,000 simulated data points on fishing
vessel location and behavior. Each observation has a target variable
`y = 'fishing' or 'not fishing'` indicating whether the vessel was
actively fishing at the time of the observation. Observations also
include a suite of predictor variables that will be used to infer
whether a vessel of unknown behavioral state was ‘fishing’ or ‘not
fishing’. These predictor variables include some time-invariant vessel
characteristics (such as vessel length), time-invariant characteristics
of the physical environment (ocean bottom depth at a particular
location), and some time-varying characteristics such as vessel speed,
vessel bearing, and time-of-day.
