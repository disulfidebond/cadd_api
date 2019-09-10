## Overview
The [Combined Annotation Dependent Depletion (CADD)](), is a useful tool for querying SNPs of interest. The following is an implementation of their API to perform batch queries.  The code is stored in this repoisitory as a jupyter notebook, which can be run by itself, or reused as part of a larger program. 

There are several important caveats to keep in mind:
* The [API](https://cadd.gs.washington.edu/api) is, by definition, experimental, and `not thought to be used for retrieving thousands or millions of variants`. Do **NOT** remove the lines of code that provide a pause, and do NOT use this for more than 1000 queries at a time. Doing so will result in the server crashing, and some very irate researchers at the University of Washington.
* The API is in the early stages, and may change significantly at a later date, requiring the code to be updated as well.
* The jupyter notebook is written to only accommodate a single SNP position, but the API also supports a SNP range, such as `22:44044001-44044002`. Modifying the code to complete this step is fairly straightforward, and has been left as an exercise to anyone so inclined.
