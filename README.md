creelSurvey
===========

*Functions to allow fisheries managers to simulate a bus route creel survey*

**This repository is no longer current.  It will be kept in place because a question on [StackOverlow.com](https://stackoverflow.com/questions/27756679/cran-finds-an-warning-that-r-cmd-check-as-cran-does-not) refers to this repository, functions, and .Rd files, but this repository will not be updated.  Please see the repository [AnglerCreelSurveySimulation](http://www.github.com/stevenranney/AnglerCreelSurveySimulation) for the most updated version of this package.**

** 2019-01-14: This repository is now read-only.**

=====
Creel surveys allow fisheries scientists and managers the ability to sample anglers in a fishery and achieve statisticaly-valid estimates of catch rate, harvest rate, and in some cases, fish populations.  Depending upon the size of the fishery, creel surveys can be challenging to implement correctly.  Further, creel surveys can be costly.  Much research has been spent on identifying methods for creel surveys.  However, relatively little research time has been spent on answering the question _what is the best creel-survey type to implement in **my** fishery?_  The package(s) and code contained in this repository include functions to allow fisheries managers the ability to simulate a creel survey with *a priori* data.

This package has been submitted to `CRAN` for publication on 4 Jan 2015.  A manuscript is in progress for publication in the Journal of Statistical Software.

Install 'AnglerCreelSurveySimulation' with
```r
install.packages("AnglerCreelSurveySimulation")
```

Additional information:
* `meanTripLength` and `catchRate` are estimated from the `gamma` distribution
* The Ratio of Means is used to estiate `catch` and `effort` (Malvestuto 1996; Jones and Pollock 2012)
* Creel surveys can be estimated as a 'one-off' or bus route-type surveys (e.g., multiple stops along a route)
* Simulations can be run to estimate `>= 1` surveys
* Resulting values for estimated catch and estimated effort can be plotted as a function of true catch and true effort to evaluate how accurately the survey reflects reality.

#####References 

Jones, C. M., and K. H. Pollock. 2012. Recreational survey 
 methods: estimation of effort, harvest, and released catch. Pages 883-919 
 in A. V. Zale, D. L. Parrish, and T. M. Sutton, editors. Fisheries 
 Techniques, 3rd edition. American Fisheries Society, Bethesda, Maryland.
 
Malvestuto, S. P. 1996. Sampling the recreational creel. Pages 
 591-623 in B. R. Murphy and D. W. Willis, editors. Fisheries techniques, 
 2nd edition. American Fisheries Society, Bethesda, Maryland.
