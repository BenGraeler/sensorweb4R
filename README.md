# sensorweb4R

R extension package to integrate sensor data into R using the [52°North Sensor Web Client API](https://wiki.52north.org/bin/view/SensorWeb/SensorWebClientRESTInterface).

[![Build Status](https://travis-ci.org/52North/sensorweb4R.png?branch=master)](https://travis-ci.org/52North/sensorweb4R)

## Installation

The sensorweb4R package is not on CRAN yet, so please download and install the package manually. The first option is using the package ``devtools``, which also works well for your own fork or development versions by other contributors.

So, if you don't have ``devtools`` installed:
```r
install.packages("devtools")
```
Continue:
```r
devtools::install_github("52North/sensorweb4R")
```
To also install the vignettes run:
```r
devtools::install_github("52North/sensorweb4R", build_vignettes = TRUE)
```

Alternatively, you can download the source code and install the package from source. For this to work must have both [git](http://git-scm.com/downloads) and R (see documentation [here](http://cran.r-project.org/bin/windows/base/rw-FAQ.html#Rcmd-is-not-found-in-my-PATH_0021) for Windows) on your path. Then run the following commands:

```shell
git clone https://github.com/52North/sensorweb4R
R CMD INSTALL sensorweb4R
```

## Documentation

Take a look at the demos to see how to use the package:

```r
library(sensorweb4R)
demo(package = "sensorweb4R")
```

For some of the demo's you will need:

```r
install.packages("maptools")
install.packages("rgdal")
```
On Fedora/RedHat/CentOS you will need the following yum packages to be able to install `rgdal`:

```shell
yum install gdal gdal-devel gdal-static proj-devel proj-epsg
```

Futher user documentation is in the R help and the vignettes:

```r
vignette(package = "sensorweb4R")
vignette("<name of the vignette to open")
```

## Development

### Building the documentation

```r
devtools::document()
```

## Contact / Support

Please direct support questions to the 52°North Sensor Web Community mailing list/forum: http://sensorweb.forum.52north.org/ (and read the [guidelines](http://52north.org/resources/mailing-list-and-forums/mailinglist-guidelines) beforehand).

Add an issue/comment on GitHub if you found a bug or want to collaborate on new features.

## License

This R extension package is licensed under [Apache License 2.0](https://www.tldrlegal.com/l/apache2).

Documentation (namely the vignettes) are published under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/).
