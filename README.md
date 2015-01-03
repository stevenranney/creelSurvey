creelSurvey
===========

*Functions to allow fisheries managers to simulate a bus route creel survey*

Creel surveys allow fisheries scientists and managers the ability to sample anglers in a fishery and achieve statisticaly-valid estimates of catch rate, harvest rate, and in some cases, fish populations.  Depending upon the size of the fishery, creel surveys can be challenging to implement correctly.  Further, creel surveys can be costly.  Much research has been spent on identifying methods for creel surveys.  However, relatively little research time has been spent on answering the question _what is the best creel-survey type to implement in **my** fishery?_  The package(s) and code contained in this repository include functions to allow fisheries managers the ability to simulate a creel survey with *a priori* data.

In the `creelSurvey` repository are two packages: `BusRouteCreelSurvey_0.1.zip` and `BusRouteCreelSurvey_0.2.zip`.  Version 0.2 is almost identical to v0.1.  The primary difference is that v0.2 has better documentation and includes references that do not appear in v0.1.  Since v0.2 was 'released,' I discovered that there are some bugs that prevent v0.2 from functioning correctly.  Specifically, passing `meanTripLength` to all functions from `SimulateBusRoute()` is challenging.  Further, in v0.3, I will include recently-acquired field data to allow users to simulate a creel survey with "real" data if they do not have their own.

Eventually, these will be published as a ShinyApp website and to CRAN, but until then, this package and its contents reside here.  Ultimately, publication of this package rests upon my ability to finish the manuscript that is in progress; target submittal date to the North American Journal of Fisheries Management is late Spring, 2015.

Additional information:
* `meanTripLength` and `catchRate` are estimated from the `gamma` distribution
* The Ratio of Means is used to estiate `catch` and `effort` (Malvestuto 1996; Jones and Pollock 2012)
* All functions were written in the format specified by the `inlinedocs` package: http://inlinedocs.r-forge.r-project.org/ which makes creation of `*.Rd` files particularly easy.

#####References 

Jones, C. M., and K. H. Pollock. 2012. Recreational survey 
 methods: estimation of effort, harvest, and released catch. Pages 883-919 
 in A. V. Zale, D. L. Parrish, and T. M. Sutton, editors. Fisheries 
 Techniques, 3rd edition. American Fisheries Society, Bethesda, Maryland.
 
Malvestuto, S. P. 1996. Sampling the recreational creel. Pages 
 591-623 in B. R. Murphy and D. W. Willis, editors. Fisheries techniques, 
 2nd edition. American Fisheries Society, Bethesda, Maryland.
