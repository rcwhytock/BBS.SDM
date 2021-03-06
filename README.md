
<!-- README.md is generated from README.Rmd. Please edit that file -->

The goal of BBS.SDM is to …

## Installation

You can install BBS.SDM from [Github](https://github.com) with:

``` r
#install.packages("devtools")
devtools::install_github("RushingLab/BBS.SDM")
```

## Additional software and packages needed

Fitting the models described in the paper requires an up-to-date version
of [JAGS](jags).

The workflow for fitting the models also relies on program
[Presence](https://www.mbr-pwrc.usgs.gov/software/presence.html), which
is called from R using the `RPresence` package (both Presence and the
binary for `RPresence` can be downloaded from the previous link). Once
downloaded, `RPresence` can be installed using the following command (be
sure to change to the correct
path\!):

``` r
install.packages("C:/path/to/file/RPresence_2.12.13.zip", repos = NULL, type = "win.binary")
```

Alternatively, if you are using RStudio, `RPresence` can be installed by
going to `Tools -> Install Packages`, clicking the `Package Archive File
(.zip; .tar.gz)` option under the `Install from:` dropdown, and then
browsing to `RPresence_2.12.13.zip` (note that the version number may be
different).

Two additional packages are needed to obtain and format the raw BBS
data. These packages can be downloaded from Github:

``` r
devtools::install_github("richfitz/datastorr")
devtools::install_github("crushing05/BBS.tenstop")
```

## Example analysis

``` r
vignette("bbs-sdm")
```
