## Update - v.0.1.7

After initial acceptance, CRAN checks identified an issue stemming from the package using a local cache that writes to the user library rather than R's temporary director. Kurt Hornik advised to fix this and to submit an update. 

* This update changes default caching behaviour to confirm with CRAN requirements. 
* Users are prompted with a suggestion encouraging them to set up a persistent local cache on load, and a second reminder when making an API call. 

## Resubmission - v.0.1.6 - Approved

This is a resubmission addressing comments from reviewer Swetlana Herbrandt. In addition to recommendations for changes to package title and description to avoid redundancy and conform to standards, Swetlana noted that all examples are wrapped in `/dontrun{}` and are not tested. 

In response, all package functions not requiring an API key to call are now tested in the documentation. All package functions including those requiring API keys are built, evaluated, and tested locally with online  [documentation](https://mountainmath.github.io/cancensus/reference/index.html). Swetlana suggested that this would be sufficient in a follow up email. 

Documentation now includes a prebuilt static html vignette rather than pdf ones to better display functionality. Package fully builds and compiles on [Travis](https://travis-ci.org/mountainMath/cancensus).

## Submission - v.0.1.6

First submission for this package. This is the first CRAN package I've developed so I apologize in advance if I have made any oversight. Thanks for your time. 

## Test environments
* local OS X install, R 3.4.3
* ubuntu 14.04 (on travis-ci), R 3.4.2
* win-builder (devel and release)

## R CMD check results
There were no ERRORs or WARNINGs and one NOTE:

 - A NOTE came up for "Maintainer:..." which I understand can be ignored

## Reverse dependencies
This is a new release and there are no dependencies.

## Vignettes
Vignettes require API authentification and code chunks are not evaluated when system variables are not enabled. Vignettes are prebuilt with pdfs included. Vignettes are evaluated locally and on Travis with [log results](https://travis-ci.org/mountainMath/cancensus).
